---
title: "Javascript Console Objects"
description: "JS is not only bounded to console.log. Explore other console objects."
pubDate: "Feb 7 2023"
heroImage: "/blog/blog-placeholder-5.jpg"
---

Here is a list of 5 console objects other than console.log that can make your debugging less frustrating and make your console beautiful.

## 1. <u>console.assert :</u>

console.assert is just like a console.log with a built in condition checker just like **if condition**. But it slightly different then traditional if condition. A tradition if condition will run a block of code if the condition is true whereas **console.assert** will log anything if the condition is false. You can compare this with the **else block**.

### Structure

```javascript
console.assert(condition, output);
```

### Example

![console.assert example](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/tvcfz8jnh7w6qbg1zymm.png)

If you don't **0.1 + 0.2 = 0.30000000000000004** in javascript due to its computing techniques

## 2. <u>console.error :</u>

console.error is really helpful when you are using multiple console.log and few of them are for just logging any value and few of them are for show any kind of error. It has different styles then normal console.log so you can easily distinguish between them the value output and errors.

### Structure

```javascript
console.error("error text which you want to log");
```

### Example

![console.error example](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/v92kez8wve9s2ps36q9j.png)

## 3. <u>console.table :</u>

console.table is very useful while working with any array or object. With this you can get a well structured table like view of your data which make it easy to read whereas console.log can make it a little bit messy.

### Structure

```javascript

console.table(object or array)


```

### Example

#### Array Output

![logging array using console.table](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/fu9c1f97b3a64ik3etrt.png)

#### Object Output

![logging object using console.table](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/17rhn0flc872c2le5gv0.png)

#### Nest Object Output

![logging nested object using console.table](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/t3rbhdyjz1b241j7f5vr.png)

It could be more messy then console.log for nested objects otherwise it's a great option for none nested objects and arrays.

## 4. <u>console.time :</u>

console.time is very very important console object which everybody should know. It can log out the time taken for running one or more block of code which has no other option than manually measuring it using an stopwatch ⏱. To use this you have wrap the block of code with **console.time()** and **console.timeEnd()**.
**console.time()** starts the timer then runs the block of code then **console.timeEnd()** stops the timer and log it in the console. It can have a argument as label for of the timer but it is not mandatory so you can skip it. But remember if you are using it both console.time() and console.timeEnd() must have same labels ohterwise it will through an error.

### Its structure

```javascript
console.time("test");
// some code which might take a time
console.timeEnd("test");
```

### Example

![console.table example](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/8ra5iwpdlckca1c16km7.png)

### For python dev

if you are know python then this is same as doing

```python

 import time

 start = time.time.time()
 do_something()
 end = time.time()
 print('time taken =>', end - start )


```

## 5. <u>console.warn :</u>

console.warn is same as console.error just the difference is it decorates the log like as a **warning ⚠ message** and console.error decorate it as error message. You can use this to log any error for your fellow programmers or future self.

### Structure

```javascript
console.warn("some warning text");
```

### Example

![console.warn example](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/4xobqnhd9aiy38a57g27.png)

## Honorable Mention

### <u>console.info :</u>

It is same as console.warn and console.error. But it is not that much decorated as those two. It only add a **i** icon before the log not much different then console.log.

![console.info example](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/xguqth4bvumt5qr8wnzn.png)

### <u>console.clear :</u>

use this to clear the console.
