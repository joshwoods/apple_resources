

- VisionKit
- VNDocumentCameraViewControllerDelegate
-  documentCameraViewController(\_:didFinishWith:) 

Instance Method

# documentCameraViewController(\_:didFinishWith:)

Tells the delegate that the user successfully saved a scanned document from the document camera.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func documentCameraViewController(
    _ controller: VNDocumentCameraViewController,
    didFinishWith scan: VNDocumentCameraScan
)
```

## Parameters 

`controller`  

The document camera view controller that captured the scan.

`scan`  

The scanned document that the camera detected.

## See Also

### Determining scan results

func documentCameraViewControllerDidCancel(VNDocumentCameraViewController)

Tells the delegate that the user canceled out of the document scanner camera.

func documentCameraViewController(VNDocumentCameraViewController, didFailWithError: any Error)

Tells the delegate that document scanning failed while the camera view controller was active.

