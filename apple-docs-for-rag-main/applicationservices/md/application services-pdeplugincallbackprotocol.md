

- Application Services
-  PDEPlugInCallbackProtocol 

Protocol

# PDEPlugInCallbackProtocol

macOS 13.0+

``` source
protocol PDEPlugInCallbackProtocol
```

## Topics

### Instance Methods

func pageFormat() -> PMPageFormat?

**Required**

func pmPrinter() -> PMPrinter

**Required**

func ppdFile() -> UnsafeMutablePointer&lt;ppd_file_s>?

**Required**

func printSession() -> PMPrintSession?

**Required**

func printSettings() -> PMPrintSettings?

**Required**

func willChangePPDOptionKeyValue(String, ppdChoice: String) -> Bool

**Required**

