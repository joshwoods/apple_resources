

- AVFoundation
- AVAssetWriter
-  init(outputURL:fileType:) 

Initializer

# init(outputURL:fileType:)

Creates an object that writes media data to a container file at the output URL.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
init(
    outputURL: URL,
    fileType outputFileType: AVFileType
) throws
```

## Parameters 

`outputURL`  

The location of the file to write.

`outputFileType`  

The type of container file to write.

## Discussion

Writing fails if a file already exists at the output URL.

## See Also

### Creating an Asset Writer

convenience init(url: URL, fileType: AVFileType) throws

Returns a new object that writes media data to a container file at the output URL.

init(contentType: UTType)

Creates an object that outputs segment data in a specified container format.

