

- VisionKit
- VNDocumentCameraViewControllerDelegate
-  documentCameraViewController(\_:didFailWithError:) 

Instance Method

# documentCameraViewController(\_:didFailWithError:)

Tells the delegate that document scanning failed while the camera view controller was active.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentCameraViewController(
    _ controller: VNDocumentCameraViewController,
    didFailWithError error: any Error
)
```

## Parameters 

`controller`  

The document camera view controller that failed.

`error`  

The error containing the reason for failure.

## See Also

### Determining scan results

func documentCameraViewController(VNDocumentCameraViewController, didFinishWith: VNDocumentCameraScan)

Tells the delegate that the user successfully saved a scanned document from the document camera.

func documentCameraViewControllerDidCancel(VNDocumentCameraViewController)

Tells the delegate that the user canceled out of the document scanner camera.

