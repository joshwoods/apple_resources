

- ReplayKit
- RPPreviewViewControllerDelegate
-  previewController(\_:didFinishWithActivityTypes:) 

Instance Method

# previewController(\_:didFinishWithActivityTypes:)

Indicates that the preview view controller is ready to be dismissed with associated activity types.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 11.0+visionOS 1.0+

``` source
optional func previewController(
    _ previewController: RPPreviewViewController,
    didFinishWithActivityTypes activityTypes: Set
)
```

**Required**

## Parameters 

`previewController`  

The preview view controller to be dismissed.

`activityTypes`  

A set of activity types as listed in UIActivity.

## Discussion

When the user is finished making changes to a screen recording, your app is responsible for dismissing the view controller representing the user interface. Call dismiss(animated:completion:) after getting the message to dismiss the preview view controller.

## See Also

### Dismissing the View Controller

func previewControllerDidFinish(RPPreviewViewController)

Indicates that the preview view controller is ready to be dismissed.

