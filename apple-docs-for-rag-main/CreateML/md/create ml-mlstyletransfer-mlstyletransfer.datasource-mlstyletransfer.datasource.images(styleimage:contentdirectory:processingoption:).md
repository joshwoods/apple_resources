

- Create ML
- MLStyleTransfer
- MLStyleTransfer.DataSource
-  MLStyleTransfer.DataSource.images(styleImage:contentDirectory:processingOption:) 

Case

# MLStyleTransfer.DataSource.images(styleImage:contentDirectory:processingOption:)

The locations of a style-image file and content-image directory in the file system.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
case images(
    styleImage: URL,
    contentDirectory: URL,
    processingOption: VNImageCropAndScaleOption? = .centerCrop
)
```

