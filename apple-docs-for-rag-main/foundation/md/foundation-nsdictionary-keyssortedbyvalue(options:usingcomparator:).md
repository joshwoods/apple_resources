

- Foundation
- NSDictionary
-  keysSortedByValue(options:usingComparator:) 

Instance Method

# keysSortedByValue(options:usingComparator:)

Returns an array of the dictionary’s keys, in the order they would be in if the dictionary were sorted by its values using a given comparator block and a specified set of options.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func keysSortedByValue(
    options opts: NSSortOptions = [],
    usingComparator cmptr: (Any, Any) -> ComparisonResult
) -> [Any]
```

## Parameters 

`opts`  

A bitmask of sort options.

`cmptr`  

A comparator block.

## Return Value

An array of the dictionary’s keys, in the order they would be in if the dictionary were sorted by its values using `cmptr` with the options given in `opts`.

## See Also

### Sorting Dictionaries

func keysSortedByValue(using: Selector) -> [Any]

Returns an array of the dictionary’s keys, in the order they would be in if the dictionary were sorted by its values.

func keysSortedByValue(comparator: (Any, Any) -> ComparisonResult) -> [Any]

Returns an array of the dictionary’s keys, in the order they would be in if the dictionary were sorted by its values using a given comparator block.

