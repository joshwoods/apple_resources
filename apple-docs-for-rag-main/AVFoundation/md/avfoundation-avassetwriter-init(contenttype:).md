

- AVFoundation
- AVAssetWriter
-  init(contentType:) 

Initializer

# init(contentType:)

Creates an object that outputs segment data in a specified container format.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
init(contentType outputContentType: UTType)
```

## Parameters 

`outputContentType`  

A type that indicates the format of the segment data to output.

## Discussion

Use this initializer to create an asset writer that outputs segment data to an adopter of the AVAssetWriterDelegate protocol. For example, you can create an asset writer object to write an MPEG-4 file as shown below:

```
// Create a UTType for the MP4 file type.
guard let contentType = UTType(AVFileType.mp4.rawValue) else { return }
let assetWriter = AVAssetWriter(contentType: contentType)
```

## See Also

### Creating an Asset Writer

convenience init(url: URL, fileType: AVFileType) throws

Returns a new object that writes media data to a container file at the output URL.

init(outputURL: URL, fileType: AVFileType) throws

Creates an object that writes media data to a container file at the output URL.

