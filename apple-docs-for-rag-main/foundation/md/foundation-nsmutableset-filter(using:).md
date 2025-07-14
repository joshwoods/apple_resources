

- Foundation
- NSMutableSet
-  filter(using:) 

Instance Method

# filter(using:)

Evaluates a given predicate against the set’s content and removes from the set those objects for which the predicate returns false.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func filter(using predicate: NSPredicate)
```

## Parameters 

`predicate`  

A predicate.

## Discussion

The following example illustrates the use of this method.

```
NSMutableSet *mutableSet =
    [NSMutableSet setWithObjects:@"One", @"Two", @"Three", @"Four", nil];
NSPredicate *predicate =
    [NSPredicate predicateWithFormat:@"SELF beginswith 'T'"];
[mutableSet filterUsingPredicate:predicate];
// mutableSet contains (Two, Three)
```

## See Also

### Adding and removing entries

func add(Any)

Adds a given object to the set, if it is not already a member.

func remove(Any)

Removes a given object from the set.

func removeAllObjects()

Empties the set of all of its members.

func addObjects(from: [Any])

Adds to the set each object contained in a given array that is not already a member.

