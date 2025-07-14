

- Objective-C Runtime
- NSObject
-  imageBrowserSelectionDidChange(\_:) 

Instance Method

# imageBrowserSelectionDidChange(\_:)

Performs custom tasks when the selection changes.

macOS

``` source
func imageBrowserSelectionDidChange(_ aBrowser: IKImageBrowserView!)
```

## Parameters 

`aBrowser`  

An image browser view.

## Discussion

This method signals that the user changes the selection in the image browser view. You can implement this method if you want to perform custom tasks at that time.

