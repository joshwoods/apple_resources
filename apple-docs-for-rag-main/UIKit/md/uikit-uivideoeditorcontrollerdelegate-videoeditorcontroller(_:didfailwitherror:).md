

- UIKit
- UIVideoEditorControllerDelegate
-  videoEditorController(\_:didFailWithError:) 

Instance Method

# videoEditorController(\_:didFailWithError:)

Notifies the delegate when the video editor is unable to load or save a movie.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func videoEditorController(
    _ editor: UIVideoEditorController,
    didFailWithError error: any Error
)
```

## Parameters 

`editor`  

The video editor that was unable to load or save a movie.

`error`  

The loading or saving error.

## Discussion

Loading a movie into the video editor could fail because of an invalid filesystem path or an invalid media format. Saving could fail because of a lack of disk space or other reasons.

