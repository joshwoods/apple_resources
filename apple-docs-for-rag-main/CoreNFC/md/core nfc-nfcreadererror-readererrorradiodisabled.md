

- Core NFC
- NFCReaderError
-  readerErrorRadioDisabled 

Type Property

# readerErrorRadioDisabled

The NFC wireless radio on the device is disabled.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static var readerErrorRadioDisabled: NFCReaderError.Code { get }
```

## Discussion

This condition happens, for example, when a person enables airplane mode on their device.

## See Also

### Other Errors

static var readerErrorUnsupportedFeature: NFCReaderError.Code

The reader session does not support this feature.

static var readerErrorInvalidParameter: NFCReaderError.Code

An input parameter is invalid.

static var readerErrorInvalidParameterLength: NFCReaderError.Code

The length of an input parameter is invalid.

static var readerErrorParameterOutOfBound: NFCReaderError.Code

A parameter value is outside of the acceptable boundary.

static var readerErrorSecurityViolation: NFCReaderError.Code

A security violation associated with the reader session has occurred.

