

- Core NFC
- NFCReaderError
-  readerErrorInvalidParameter 

Type Property

# readerErrorInvalidParameter

An input parameter is invalid.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
static var readerErrorInvalidParameter: NFCReaderError.Code { get }
```

## See Also

### Other Errors

static var readerErrorUnsupportedFeature: NFCReaderError.Code

The reader session does not support this feature.

static var readerErrorInvalidParameterLength: NFCReaderError.Code

The length of an input parameter is invalid.

static var readerErrorParameterOutOfBound: NFCReaderError.Code

A parameter value is outside of the acceptable boundary.

static var readerErrorRadioDisabled: NFCReaderError.Code

The NFC wireless radio on the device is disabled.

static var readerErrorSecurityViolation: NFCReaderError.Code

A security violation associated with the reader session has occurred.

