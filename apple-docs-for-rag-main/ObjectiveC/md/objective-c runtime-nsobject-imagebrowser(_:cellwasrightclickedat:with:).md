

- Objective-C Runtime
- NSObject
-  imageBrowser(\_:cellWasRightClickedAt:with:) 

Instance Method

# imageBrowser(\_:cellWasRightClickedAt:with:)

Performs custom tasks when the user right-clicks an item in the image browser view.

macOS

``` source
func imageBrowser(
    _ aBrowser: IKImageBrowserView!,
    cellWasRightClickedAt index: Int,
    with event: NSEvent!
)
```

## Parameters 

`aBrowser`  

An image browser view.

`index`  

The index of the cell.

`event`  

The event that invoked the method.

## Discussion

This method signals that the user either right-clicked an item in the browser or left-clicked the item with the Alt key pressed. You can implement this method if you want to perform custom tasks at that time.

