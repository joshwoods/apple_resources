

- UIKit
- UILocalizedIndexedCollation
-  sortedArray(from:collationStringSelector:) 

Instance Method

# sortedArray(from:collationStringSelector:)

Sorts the objects within a section by their localized titles.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func sortedArray(
    from array: [Any],
    collationStringSelector selector: Selector
) -> [Any]
```

## Parameters 

`array`  

An array containing the model objects for a section.

`selector`  

The selector of a method implemented by the objects in `array` that returns the string to use for sorting the objects. The method represented by the selector must take no arguments and return an NSString object. For example, you might specify the selector for a name property of the object.

## Return Value

A new array containing the sorted items from the original `array` parameter.

## Discussion

The table-view controller creates the array of objects for a section (`array`) as part of iterating through its model objects with calls to the section(for:collationStringSelector:) method. This method should be called on each local section array.

## See Also

### Preparing the sections and section indexes

func section(for: Any, collationStringSelector: Selector) -> Int

Returns an integer identifying the section in which a model object belongs.

