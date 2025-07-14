

- VisionKit
- VNDocumentCameraViewController
-  isSupported 

Type Property

# isSupported

A Boolean variable that indicates whether or not the current device supports document scanning.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class var isSupported: Bool { get }
```

## Discussion

This class method returns `false` for unsupported hardware.

## See Also

### Supporting the document camera

var delegate: (any VNDocumentCameraViewControllerDelegate)?

The delegate to be notified when the user saves or cancels the document scanner.

