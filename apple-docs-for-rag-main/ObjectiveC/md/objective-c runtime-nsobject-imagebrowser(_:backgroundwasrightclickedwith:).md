

- Objective-C Runtime
- NSObject
-  imageBrowser(\_:backgroundWasRightClickedWith:) 

Instance Method

# imageBrowser(\_:backgroundWasRightClickedWith:)

Performs custom tasks when the user right-clicks the image browser view background.

macOS

``` source
func imageBrowser(
    _ aBrowser: IKImageBrowserView!,
    backgroundWasRightClickedWith event: NSEvent!
)
```

## Parameters 

`aBrowser`  

An image browser view.

`event`  

The event that invoked the method.

## Discussion

This method signals that the user either right-clicked the background or left-clicked it with the Alt key pressed. You can implement this method if you want to perform custom tasks at that time.

