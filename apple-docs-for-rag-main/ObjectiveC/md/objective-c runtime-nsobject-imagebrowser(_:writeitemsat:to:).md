

- Objective-C Runtime
- NSObject
-  imageBrowser(\_:writeItemsAt:to:) 

Instance Method

# imageBrowser(\_:writeItemsAt:to:)

Signals that a drag should begin.

macOS

``` source
func imageBrowser(
    _ aBrowser: IKImageBrowserView!,
    writeItemsAt itemIndexes: IndexSet!,
    to pasteboard: NSPasteboard!
) -> Int
```

## Parameters 

`aBrowser`  

An image browser view.

`itemIndexes`  

The indexes of the items that should be dragged.

`pasteboard`  

The pasteboard to copy the items to.

## Return Value

The number of items written to the pasteboard.

## Discussion

This method is optional. It is invoked after Image Kit determines that a drag should begin, but before the drag has been started.

