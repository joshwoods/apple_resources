

- AVFoundation
- AVCaptureMetadataOutput
-  availableMetadataObjectTypes 

Instance Property

# availableMetadataObjectTypes

An array of strings identifying the types of metadata objects that can be captured.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 13.0+tvOS 17.0+

``` source
var availableMetadataObjectTypes: [AVMetadataObject.ObjectType] { get }
```

## Discussion

Each string in the array corresponds to a possible value in the type property of the AVMetadataObject objects reported by the receiver. The available types are dependent on the capabilities of the AVCaptureInput.Port to which the receiver’s connection is attached.

## See Also

### Configuring Metadata Capture

var metadataObjectTypes: [AVMetadataObject.ObjectType]!

An array of strings identifying the types of metadata objects to process.

var rectOfInterest: CGRect

A rectangle of interest for limiting the search area for visual metadata.

