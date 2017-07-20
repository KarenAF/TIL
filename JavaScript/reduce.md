7/19/17 Javascript method: Reduce

How to get the average of an array of numbers using the Reduce method:

Similar to Ruby's method of Inject(+), C# Enumerable.Aggregate, and Python reduce, Reduce is a method that 'reduces' each iterated value in an iterable (e.g. array) down to one value. In other words, it applies the function to the left argument x, and right argument, y.

It is written as such:
```
var array = [1, 2, 3, 4, 5, 6];

average = array.reduce((x, y) =>
    x + y)/array.length;

console.log(average);

```

