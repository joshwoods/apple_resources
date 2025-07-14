

- UIKit
- UILocalizedIndexedCollation
-  section(for:collationStringSelector:) 

Instance Method

# section(for:collationStringSelector:)

Returns an integer identifying the section in which a model object belongs.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func section(
    for object: Any,
    collationStringSelector selector: Selector
) -> Int
```

## Parameters 

`object`  

A model object of the application that is part of the data model for the table view.

`selector`  

The selector of a method of `object` that returns the string to use for sorting. The method represented by the selection must take no arguments and return an NSString object. For example, you might specify the selector for a `name` property of the object.

## Return Value

An integer that identifies the section in which the model object belongs. The numbers returned indicate a sequential ordering.

## Discussion

The table-view controller should iterate through all model objects for the table view and call this method for each object. If the application provides a `Localizable.strings` file for the current language preference, the indexed-collation object localizes each string returned by the method identified by `selector`. It uses this localized name when collating titles. The controller should use the returned integer to identify a local “section” array in which it should insert `object`.

## See Also

### Preparing the sections and section indexes

func sortedArray(from: [Any], collationStringSelector: Selector) -> [Any]

Sorts the objects within a section by their localized titles.

