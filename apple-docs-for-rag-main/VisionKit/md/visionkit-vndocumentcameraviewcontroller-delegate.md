

- VisionKit
- VNDocumentCameraViewController
-  delegate 

Instance Property

# delegate

The delegate to be notified when the user saves or cancels the document scanner.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any VNDocumentCameraViewControllerDelegate)? { get set }
```

## Overview

The delegate receives one of the following three calls:

- documentCameraViewController(_:didFinishWith:) when the camera successfully completes a scan.

- documentCameraViewControllerDidCancel(_:) when the user cancels out of the document camera interface.

- documentCameraViewController(_:didFailWithError:) when the document scan fails or is unable to capture a photo.

Your app is responsible for dismissing the document camera in all delegate methods.

## See Also

### Supporting the document camera

class var isSupported: Bool

A Boolean variable that indicates whether or not the current device supports document scanning.

