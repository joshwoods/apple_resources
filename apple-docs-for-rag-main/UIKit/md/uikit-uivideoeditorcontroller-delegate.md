

- UIKit
- UIVideoEditorController
-  delegate 

Instance Property

# delegate

The video editor’s delegate object.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
unowned(unsafe) var delegate: (any UINavigationControllerDelegate & UIVideoEditorControllerDelegate)? { get set }
```

## Discussion

The delegate receives a notification when the system has finished saving an edited movie or when the user cancels the video editor. The delegate also decides when to dismiss the editor interface, so you must provide a delegate to use a video editor. If this property is `nil`, the editor is dismissed immediately if you try to show it. The delegate protocol is described in UIVideoEditorControllerDelegate.

## See Also

### Managing changes to the video

protocol UIVideoEditorControllerDelegate

A set of methods that your delegate object must implement to respond to the video editor.

