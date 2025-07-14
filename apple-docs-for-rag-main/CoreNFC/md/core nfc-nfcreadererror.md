

- Core NFC
-  NFCReaderError 

Structure

# NFCReaderError

An error type that indicates problems with reader sessions or tags.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
struct NFCReaderError
```

## Topics

### Session Errors

static var readerSessionInvalidationErrorFirstNDEFTagRead: NFCReaderError.Code

The first NDEF tag read by this session is invalid.

static var readerSessionInvalidationErrorSessionTerminatedUnexpectedly: NFCReaderError.Code

The reader session terminated unexpectedly.

static var readerSessionInvalidationErrorSessionTimeout: NFCReaderError.Code

The reader session timed out.

static var readerSessionInvalidationErrorSystemIsBusy: NFCReaderError.Code

The reader session failed because the system is busy.

static var readerSessionInvalidationErrorUserCanceled: NFCReaderError.Code

The user canceled the reader session.

### NDEF Tag Errors

static var ndefReaderSessionErrorTagNotWritable: NFCReaderError.Code

The NDEF tag isn’t writable.

static var ndefReaderSessionErrorTagSizeTooSmall: NFCReaderError.Code

The NDEF tag memory size is too small to store the data.

static var ndefReaderSessionErrorTagUpdateFailure: NFCReaderError.Code

The reader session failed to update the NDEF tag.

static var ndefReaderSessionErrorZeroLengthMessage: NFCReaderError.Code

The NDEF tag doesn’t contain an NDEF message.

### Transceive Errors

static var readerTransceiveErrorRetryExceeded: NFCReaderError.Code

Too many retries have occurred.

static var readerTransceiveErrorTagConnectionLost: NFCReaderError.Code

The reader lost the connection to the tag.

static var readerTransceiveErrorTagNotConnected: NFCReaderError.Code

The tag isn’t in the connected state.

static var readerTransceiveErrorTagResponseError: NFCReaderError.Code

The tag has responded with an error.

static var readerTransceiveErrorSessionInvalidated: NFCReaderError.Code

The reader session is invalid.

static var readerTransceiveErrorPacketTooLong: NFCReaderError.Code

The packet length exceeds the limit supported by the tag.

### Tag Command Configuration Error

static var tagCommandConfigurationErrorInvalidParameters: NFCReaderError.Code

The tag has been configured with invalid parameters.

### Other Errors

static var readerErrorUnsupportedFeature: NFCReaderError.Code

The reader session does not support this feature.

static var readerErrorInvalidParameter: NFCReaderError.Code

An input parameter is invalid.

static var readerErrorInvalidParameterLength: NFCReaderError.Code

The length of an input parameter is invalid.

static var readerErrorParameterOutOfBound: NFCReaderError.Code

A parameter value is outside of the acceptable boundary.

static var readerErrorRadioDisabled: NFCReaderError.Code

The NFC wireless radio on the device is disabled.

static var readerErrorSecurityViolation: NFCReaderError.Code

A security violation associated with the reader session has occurred.

### Error Domain

let NFCErrorDomain: String

The domain for errors associated with Core NFC APIs.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

enum Code

Reader session and tag error codes.

let NFCErrorDomain: String

The domain for errors associated with Core NFC APIs.

let NFCTagResponseUnexpectedLengthErrorKey: String

A user-information dictionary key that indicates an invalid received response packet length.

