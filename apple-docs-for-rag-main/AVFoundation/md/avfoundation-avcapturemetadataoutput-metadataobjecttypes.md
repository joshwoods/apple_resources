

- AVFoundation
- AVCaptureMetadataOutput
-  metadataObjectTypes 

Instance Property

# metadataObjectTypes

An array of strings identifying the types of metadata objects to process.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 13.0+tvOS 17.0+

``` source
var metadataObjectTypes: [AVMetadataObject.ObjectType]! { get set }
```

## Discussion

This property is used to filter the metadata objects reported by the receiver. Only metadata objects whose type matches one of the strings in this property are forwarded to the delegate’s metadataOutput(_:didOutput:from:) method for processing.

When assigning a new array to this property, each of the type strings must be present in the array returned by the availableMetadataObjectTypes property; otherwise, the receiver raises anNSException.

The default is an empty NSArray object, and as a result, no metadata objects are forwarded to the delegate’s metadataOutput(_:didOutput:from:) method. The same result can be achieved by setting the property to `nil`. This default behavior maximizes both performance and battery life.

Note

Applications linked prior to iOS 7.0 will pass AVMetadataFaceObject objects to the delegate by default, if supported by the device.

## See Also

### Configuring Metadata Capture

var availableMetadataObjectTypes: [AVMetadataObject.ObjectType]

An array of strings identifying the types of metadata objects that can be captured.

var rectOfInterest: CGRect

A rectangle of interest for limiting the search area for visual metadata.

