

- Quick Look
- PreviewApplication
-  open(items:selectedItem:) 

Type Method

# open(items:selectedItem:)

Previews the provided items.

visionOS 2.0+

``` source
final class func open(
    items: [PreviewItem],
    selectedItem: PreviewItem? = nil
) -> PreviewSession
```

## Parameters 

`items`  

An array of preview items to present in the new `PreviewApplication` scene.

`selectedItem`  

If provided and in the array of passed items, the preview item to select in the presented collection..

## Return Value

A `PreviewSession` instance.

## Discussion

This method launches the preview application with the provided preview items and, optionally, a selected item.

