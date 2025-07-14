

- UIKit
- UIVideoEditorControllerDelegate
-  videoEditorController(\_:didSaveEditedVideoToPath:) 

Instance Method

# videoEditorController(\_:didSaveEditedVideoToPath:)

Notifies the delegate after the system finishes saving an edited movie.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func videoEditorController(
    _ editor: UIVideoEditorController,
    didSaveEditedVideoToPath editedVideoPath: String
)
```

## Parameters 

`editor`  

The video editor that has finished editing and saving a movie.

`editedVideoPath`  

The filesystem path to the edited movie.

## See Also

### Closing the video editor

func videoEditorControllerDidCancel(UIVideoEditorController)

Notifies the delegate when the user cancels a movie editing operation.

