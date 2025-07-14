

- AVFoundation
- AVAssetReaderOutputCaptionAdaptor
-  validationDelegate 

Instance Property

# validationDelegate

A delegate object that handles callbacks to the caption adaptor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
weak var validationDelegate: (any AVAssetReaderCaptionValidationHandling)? { get set }
```

## See Also

### Managing the Validation Delegate

protocol AVAssetReaderCaptionValidationHandling

A protocol that defines the methods for caption validation events.

