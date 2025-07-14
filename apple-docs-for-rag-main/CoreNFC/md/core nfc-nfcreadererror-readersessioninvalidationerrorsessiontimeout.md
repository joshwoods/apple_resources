

- Core NFC
- NFCReaderError
-  readerSessionInvalidationErrorSessionTimeout 

Type Property

# readerSessionInvalidationErrorSessionTimeout

The reader session timed out.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
static var readerSessionInvalidationErrorSessionTimeout: NFCReaderError.Code { get }
```

## See Also

### Session Errors

static var readerSessionInvalidationErrorFirstNDEFTagRead: NFCReaderError.Code

The first NDEF tag read by this session is invalid.

static var readerSessionInvalidationErrorSessionTerminatedUnexpectedly: NFCReaderError.Code

The reader session terminated unexpectedly.

static var readerSessionInvalidationErrorSystemIsBusy: NFCReaderError.Code

The reader session failed because the system is busy.

static var readerSessionInvalidationErrorUserCanceled: NFCReaderError.Code

The user canceled the reader session.

