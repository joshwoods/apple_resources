

- Video Toolbox
-  kVTCompressionPropertyKey_PixelTransferProperties 

Global Variable

# kVTCompressionPropertyKey_PixelTransferProperties

Properties for configuring a pixel transfer session.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_PixelTransferProperties: CFString
```

## Discussion

The properties for configuring a VTPixelTransferSession to transfer source frames from the client’s image buffers to the video encoder’s image buffers, if necessary.

## Discussion

The value is a doc://com.apple.documentation/documentation/corefoundation/cfdictionary-rum of properties to configure a VTPixelTransferSession. Setting this property alone does not necessarily guarantee that a VTPixelTransferSession will be created.

