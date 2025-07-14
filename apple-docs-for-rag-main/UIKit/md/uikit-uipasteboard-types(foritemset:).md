

- UIKit
- UIPasteboard
-  types(forItemSet:) 

Instance Method

# types(forItemSet:)

Returns an array of representation types for each specified pasteboard item.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func types(forItemSet itemSet: IndexSet?) -> [[String]]?
```

## Parameters 

`itemSet`  

An index set with each integer value identifying a pasteboard item positionally in the pasteboard. Pass in `nil` to request all pasteboard items.

## Return Value

An array of arrays, with each inner array holding the representation types for a particular pasteboard item.

## See Also

### Related Documentation

var numberOfItems: Int

The number of items for the pasteboard.

### Determining types of pasteboard items

var types: [String]

The types of the first item on the pasteboard.

func contains(pasteboardTypes: [String]) -> Bool

Returns whether the pasteboard holds data of the specified representation type.

func contains(pasteboardTypes: [String], inItemSet: IndexSet?) -> Bool

Returns whether the specified pasteboard items contain data of the given representation types.

func itemSet(withPasteboardTypes: [String]) -> IndexSet?

Returns an index set identifying pasteboard items having the specified representation types.

