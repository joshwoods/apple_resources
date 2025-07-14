

- UIKit
- UIVideoEditorControllerDelegate
-  videoEditorControllerDidCancel(\_:) 

Instance Method

# videoEditorControllerDidCancel(\_:)

Notifies the delegate when the user cancels a movie editing operation.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func videoEditorControllerDidCancel(_ editor: UIVideoEditorController)
```

## Parameters 

`editor`  

The video editor that the user canceled, not wanting to save changes.

## See Also

### Closing the video editor

func videoEditorController(UIVideoEditorController, didSaveEditedVideoToPath: String)

Notifies the delegate after the system finishes saving an edited movie.

