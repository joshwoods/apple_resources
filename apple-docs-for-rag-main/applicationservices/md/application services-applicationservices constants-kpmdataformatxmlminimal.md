

- Application Services
- ApplicationServices Constants
-  kPMDataFormatXMLMinimal 

Global Variable

# kPMDataFormatXMLMinimal

macOS 10.5+

``` source
var kPMDataFormatXMLMinimal: PMDataFormat { get }
```

## Discussion

Specifies an uncompressed data format that is approximately 3-5 times smaller than `kPMDataFormatXMLDefault`. This data format is only compatible with macOS 10.5 and later. This format is a good choice when you do not need to use the data in versions of macOS prior to 10.5 and you need a pure XML representation of the data.

