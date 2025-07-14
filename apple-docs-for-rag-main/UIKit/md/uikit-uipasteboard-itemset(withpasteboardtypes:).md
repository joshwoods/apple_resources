

- UIKit
- UIPasteboard
-  itemSet(withPasteboardTypes:) 

Instance Method

# itemSet(withPasteboardTypes:)

Returns an index set identifying pasteboard items having the specified representation types.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func itemSet(withPasteboardTypes pasteboardTypes: [String]) -> IndexSet?
```

## Parameters 

`pasteboardTypes`  

An array of strings, with each string identifying a representation type. Typically you use UTIs as pasteboard types.

## Return Value

An index set with each integer positionally identifying a pasteboard item that has one of the representation types specified in `pasteboardTypes`.

## Discussion

You can pass the index set returned in this method in a call to data(forPasteboardType:inItemSet:) or values(forPasteboardType:inItemSet:) to get the data in the indicated pasteboard items.

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

func contains(pasteboardTypes: [String], inItemSet: IndexSet?) -> Bool

Returns whether the specified pasteboard items contain data of the given representation types.

