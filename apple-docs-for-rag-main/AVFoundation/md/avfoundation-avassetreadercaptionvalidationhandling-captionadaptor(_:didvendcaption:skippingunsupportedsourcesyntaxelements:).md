

- AVFoundation
- AVAssetReaderCaptionValidationHandling
-  captionAdaptor(\_:didVendCaption:skippingUnsupportedSourceSyntaxElements:) 

Instance Method

# captionAdaptor(\_:didVendCaption:skippingUnsupportedSourceSyntaxElements:)

Tells the delegate that the adaptor ignored one or more syntax elements when it created the caption object.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
optional func captionAdaptor(
    _ adaptor: AVAssetReaderOutputCaptionAdaptor,
    didVendCaption caption: AVCaption,
    skippingUnsupportedSourceSyntaxElements syntaxElements: [String]
)
```

## Parameters 

`adaptor`  

The adaptor object.

`caption`  

The vended caption.

`syntaxElements`  

The array of unsupported syntax elements that the adaptor object skipped.

