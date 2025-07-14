

- AVFoundation
-  AVAssetReaderCaptionValidationHandling 

Protocol

# AVAssetReaderCaptionValidationHandling

A protocol that defines the methods for caption validation events.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
protocol AVAssetReaderCaptionValidationHandling : NSObjectProtocol
```

## Topics

### Validating Captions

func captionAdaptor(AVAssetReaderOutputCaptionAdaptor, didVendCaption: AVCaption, skippingUnsupportedSourceSyntaxElements: [String])

Tells the delegate that the adaptor ignored one or more syntax elements when it created the caption object.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing the Validation Delegate

var validationDelegate: (any AVAssetReaderCaptionValidationHandling)?

A delegate object that handles callbacks to the caption adaptor.

