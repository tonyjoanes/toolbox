# LINQ Examples and Explanations

Language integrated query can be used for writing queries against strongly typed collections.



## Select

## Where

## OrderBy

## Zip

## Aggregate

To understand a definition of Aggregate think of it in terms of
performing an operation on each element of the list taking 
into account the previous operations. 
That is to say it performs the action on the first and second 
element and carries the result forward. 
Then it operates on the previous result and the third element 
and carries forward. etc.

You can use aggregate to sum up numbers in a collection. 
Note here that we have an accumulated value and the next value
in the lambda.

```csharp
var nums = new[] { 1, 2, 3, 4 };
var sum = nums.Aggregate((accumulated, next) => accumulated + next);
Console.WriteLine(sum); // output: 10 (1+2+3+4)
```

## Count

```csharp
IEnumerable<string> items = new List<string> { "A", "B", "C" };
int count = items.Count();  // count: 3
```

You can use count with predicates

```csharp
IEnumerable<int> items = new List<int> { 8, 3, 2 };

// these two lines do the same
int count = items.Where(x => x < 5).Count();  // count: 2
int count = items.Count(x => x < 5);          // count: 2

// you can apply functions in the predicate too
IEnumerable<string> strings = new List<string> { "first", "then", "and then", "finally" };
// Will return 2
int result = strings.Count(str => str.Contains("then"));
```

Example with Linq extension method and with query objects

```csharp
int[] intNumbers = new int[] { 60, 80, 50, 90, 10, 30, 70, 40, 20, 100 };
            //Using Method Syntax
            int MSCount = intNumbers.Count();
            
            //Using Query Syntax
            int QSCount = (from num in intNumbers
                                    select num).Count();
```