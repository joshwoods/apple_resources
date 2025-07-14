

- AVFoundation
-  AVVideoEncoderSpecificationKey 

Global Variable

# AVVideoEncoderSpecificationKey

The video encoder specification includes options for choosing a specific video encoder.

macOS 10.10+

``` source
let AVVideoEncoderSpecificationKey: String
```

## Discussion

The value for this key is a dictionary containing `kVTVideoEncoderSpecification_*` keys specified in the VideoToolbox framework. This key should be specified at the top level of an `AVVideoSettings` dictionary.

