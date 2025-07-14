

- VisionKit
- VNDocumentCameraViewControllerDelegate
-  documentCameraViewControllerDidCancel(\_:) 

Instance Method

# documentCameraViewControllerDidCancel(\_:)

Tells the delegate that the user canceled out of the document scanner camera.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentCameraViewControllerDidCancel(_ controller: VNDocumentCameraViewController)
```

## Parameters 

`controller`  

The document camera view controller in which the user canceled.

## See Also

### Determining scan results

func documentCameraViewController(VNDocumentCameraViewController, didFinishWith: VNDocumentCameraScan)

Tells the delegate that the user successfully saved a scanned document from the document camera.

func documentCameraViewController(VNDocumentCameraViewController, didFailWithError: any Error)

Tells the delegate that document scanning failed while the camera view controller was active.

