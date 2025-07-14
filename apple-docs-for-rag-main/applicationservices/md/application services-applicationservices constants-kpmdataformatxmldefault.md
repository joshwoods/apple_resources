

- Application Services
- ApplicationServices Constants
-  kPMDataFormatXMLDefault 

Global Variable

# kPMDataFormatXMLDefault

macOS 10.5+

``` source
var kPMDataFormatXMLDefault: PMDataFormat { get }
```

## Discussion

Specifies a data format that is compatible with all macOS versions. Data in this format can be used with the `PMUnflattenXXX` functions present in versions of macOS prior to 10.5. This format is a pure XML representation of the data. However, this format is much larger than the more modern data formats described below.

