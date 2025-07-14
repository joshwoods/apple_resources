

- AVFoundation
- AVTimedMetadataGroup
-  copyFormatDescription() 

Instance Method

# copyFormatDescription()

Creates a format description based on the receiver’s items.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func copyFormatDescription() -> CMMetadataFormatDescription?
```

## Return Value

An instance of CMMetadataFormatDescription sufficient to describe the contents of all the items referenced by the object.

## Discussion

The returned format description is suitable for use as the format hint parameter when creating an instance of AVAssetWriterInput.

Each item referenced by the receiver must carry a non-`nil` value for its `dataType` property. An exception will be thrown if any item does not have a data type.

