

- UIKit
- UIPasteboard
-  contains(pasteboardTypes:inItemSet:) 

Instance Method

# contains(pasteboardTypes:inItemSet:)

Returns whether the specified pasteboard items contain data of the given representation types.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func contains(
    pasteboardTypes: [String],
    inItemSet itemSet: IndexSet?
) -> Bool
```

## Parameters 

`pasteboardTypes`  

An array of strings, with each string identifying a representation type. Typically you use UTIs as pasteboard types.

`itemSet`  

An index set with each integer value identifying a pasteboard item positionally in the pasteboard. Pass in `nil` to request all pasteboard items.

## Return Value

true if the pasteboard items identified by `itemSet` have data corresponding to the representation types specified by `pasteboardTypes`; otherwise, returns false.

## See Also

### Related Documentation

var numberOfItems: Int

The number of items for the pasteboard.

### Determining types of pasteboard items

var types: [String]

The types of the first item on the pasteboard.

func types(forItemSet: IndexSet?) -> [[String]]?

Returns an array of representation types for each specified pasteboard item.

func contains(pasteboardTypes: [String]) -> Bool

Returns whether the pasteboard holds data of the specified representation type.

func itemSet(withPasteboardTypes: [String]) -> IndexSet?

Returns an index set identifying pasteboard items having the specified representation types.

