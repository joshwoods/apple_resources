

- Objective-C Runtime
- NSObject
-  imageBrowser(\_:cellWasDoubleClickedAt:) 

Instance Method

# imageBrowser(\_:cellWasDoubleClickedAt:)

Performs custom tasks when the user double-clicks an item in the image browser view.

macOS

``` source
func imageBrowser(
    _ aBrowser: IKImageBrowserView!,
    cellWasDoubleClickedAt index: Int
)
```

## Parameters 

`aBrowser`  

An image browser view.

`index`  

The index of the cell.

## Discussion

This method signals that the user double-clicked an item in the image browser view. You can implement this method if you want to perform custom tasks at that time.

