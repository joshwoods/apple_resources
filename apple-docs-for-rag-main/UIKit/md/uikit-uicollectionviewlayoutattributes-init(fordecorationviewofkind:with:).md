

- UIKit
- UICollectionViewLayoutAttributes
-  init(forDecorationViewOfKind:with:) 

Initializer

# init(forDecorationViewOfKind:with:)

Creates and returns a layout attributes object that represents the specified decoration view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
convenience init(
    forDecorationViewOfKind decorationViewKind: String,
    with indexPath: IndexPath
)
```

## Parameters 

`decorationViewKind`  

The kind identifier for the specified decoration view.

`indexPath`  

An index path related to the decoration view.

## Return Value

A new layout attributes object whose precise type matches the type of the class used to call this method.

## Discussion

Use this method to create a layout attributes object for a decoration view in the collection view. Decoration views are a type of supplementary view but do not present data that is managed by the collection view’s data source. Instead, they mostly present visual adornments for a section or for the entire collection view.

It is up to you to decide how to use the `indexPath` parameter to identify a given decoration view. Typically, you use the `decorationViewKind` parameter to identify the type of the decoration view and the `indexPath` information to distinguish between different instances of that view.

## See Also

### Creating layout attributes

convenience init(forCellWith: IndexPath)

Creates and returns a layout attributes object that represents a cell with the specified index path.

convenience init(forSupplementaryViewOfKind: String, with: IndexPath)

Creates and returns a layout attributes object that represents the specified supplementary view.

