

- Core NFC
- NFCReaderError
-  readerSessionInvalidationErrorSessionTerminatedUnexpectedly 

Type Property

# readerSessionInvalidationErrorSessionTerminatedUnexpectedly

The reader session terminated unexpectedly.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
static var readerSessionInvalidationErrorSessionTerminatedUnexpectedly: NFCReaderError.Code { get }
```

## See Also

### Session Errors

static var readerSessionInvalidationErrorFirstNDEFTagRead: NFCReaderError.Code

The first NDEF tag read by this session is invalid.

static var readerSessionInvalidationErrorSessionTimeout: NFCReaderError.Code

The reader session timed out.

static var readerSessionInvalidationErrorSystemIsBusy: NFCReaderError.Code

The reader session failed because the system is busy.

static var readerSessionInvalidationErrorUserCanceled: NFCReaderError.Code

The user canceled the reader session.

