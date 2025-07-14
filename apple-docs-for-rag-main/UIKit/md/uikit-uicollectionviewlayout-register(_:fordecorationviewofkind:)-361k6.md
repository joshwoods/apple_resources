

- UIKit
- UICollectionViewLayout
-  register(\_:forDecorationViewOfKind:) 

Instance Method

# register(\_:forDecorationViewOfKind:)

Registers a class for use in creating decoration views for a collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func register(
    _ viewClass: AnyClass?,
    forDecorationViewOfKind elementKind: String
)
```

## Parameters 

`viewClass`  

The class to use for the supplementary view.

`elementKind`  

The element kind of the decoration view. You can use this string to distinguish between decoration views with different purposes in the layout. This parameter must not be `nil` and must not be an empty string.

## Discussion

This method gives the layout object a chance to register a decoration view for use in the collection view. Decoration views provide visual adornments to a section or to the entire collection view but are not otherwise tied to the data provided by the collection view’s data source.

You do not need to create decoration views explicitly. After registering one, it is up to the layout object to decide when a decoration view is needed and return the corresponding layout attributes from its layoutAttributesForElements(in:) method. For layout attributes that specify a decoration view, the collection view creates (or reuses) a view and displays it automatically based on the registered information.

If you previously registered a class or nib file with the same kind string, the class you specify in the `viewClass` parameter replaces the old entry. You may specify `nil` for `viewClass` if you want to unregister the decoration view.

## See Also

### Registering decoration views

func register(UINib?, forDecorationViewOfKind: String)

Registers a nib file for use in creating decoration views for a collection view.

