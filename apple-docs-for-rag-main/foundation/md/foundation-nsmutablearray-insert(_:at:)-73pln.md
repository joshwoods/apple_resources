

- Foundation
- NSMutableArray
-  insert(\_:at:) 

Instance Method

# insert(\_:at:)

Inserts the objects in the provided array into the receiving array at the specified indexes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func insert(
    _ objects: [Any],
    at indexes: IndexSet
)
```

## Parameters 

`objects`  

An array of objects to insert into the receiving array.

`indexes`  

The indexes at which the objects in `objects` should be inserted. The count of locations in `indexes` must equal the count of `objects`. For more details, see the Discussion.

## Discussion

Each object in `objects` is inserted into the receiving array in turn at the corresponding location specified in `indexes` after earlier insertions have been made. The implementation is conceptually similar to that illustrated in the following example:

```
- void insertObjects:(NSArray *)additions atIndexes:(NSIndexSet *)indexes
{
    NSUInteger currentIndex = [indexes firstIndex];
    NSUInteger i, count = [indexes count];

    for (i = 0; i 

The resulting behavior is illustrated by the following example:

```
NSMutableArray *array = [NSMutableArray arrayWithObjects: @"one", @"two", @"three", @"four", nil];
NSArray *newAdditions = [NSArray arrayWithObjects: @"a", @"b", nil];
NSMutableIndexSet *indexes = [NSMutableIndexSet indexSetWithIndex:1];
[indexes addIndex:3];
[array insertObjects:newAdditions atIndexes:indexes];
NSLog(@"array: %@", array);

// Output: array: (one, a, two, b, three, four)
```

The locations specified by `indexes` may therefore only exceed the bounds of the receiving array if one location specifies the count of the array or the count of the array after preceding insertions, and other locations exceeding the bounds do so in a contiguous fashion from that location, as illustrated in the following examples.

In this example, both new objects are appended to the end of the array.

```
NSMutableArray *array = [NSMutableArray arrayWithObjects: @"one", @"two", @"three", @"four", nil];
NSArray *newAdditions = [NSArray arrayWithObjects: @"a", @"b", nil];
NSMutableIndexSet *indexes = [NSMutableIndexSet indexSetWithIndex:5];
[indexes addIndex:4];
[array insertObjects:newAdditions atIndexes:indexes];
NSLog(@"array: %@", array);

// Output: array: (one, two, three, four, a, b)
```

If you replace `[indexes addIndex:4]` with `[indexes addIndex:6]` (so that the indexes are 5 and 6), then the application will fail with an out of bounds exception.

In this example, two objects are added into the middle of the array, and another at the current end of the array (index 4) which means that it is third from the end of the modified array.

```
NSMutableArray *array = [NSMutableArray arrayWithObjects: @"one", @"two", @"three", @"four", nil];
NSArray *newAdditions = [NSArray arrayWithObjects: @"a", @"b", @"c", nil];
NSMutableIndexSet *indexes = [NSMutableIndexSet indexSetWithIndex:1];
[indexes addIndex:2];
[indexes addIndex:4];
[array insertObjects:newAdditions atIndexes:indexes];
NSLog(@"array: %@", array);

// Output: array: (one, a, b, two, c, three, four)
```

If you replace `[indexes addIndex:4]` with `[indexes addIndex:6]` (so that the indexes are 1, 2, and 6), then the output is `(one, a, b, two, three, four, c)`.

If `objects` or `indexes` is `nil`, this method will raises an exception.

## See Also

### Adding Objects

func add(Any)

Inserts a given object at the end of the array.

func addObjects(from: [Any])

Adds the objects contained in another given array to the end of the receiving array’s content.

func insert(Any, at: Int)

Inserts a given object into the array’s contents at a given index.

