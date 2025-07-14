

- Quick Look
- QLPreviewReply
-  init(fileURL:) 

Initializer

# init(fileURL:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
init(fileURL: URL)
```

## Parameters 

`fileURL`  

A file URL representing a preview of the previewed URL. Currently supported types include: UTTypeImage, UTTypePDF, UTTypeHTML, UTTypeXML, UTTypePlainText, UTTypeRTF, UTTypeRTFD, UTTypeMovie, UTTypeAudio

## Discussion

Use this method to provide a preview by providing a URL to a file of a supported type.

