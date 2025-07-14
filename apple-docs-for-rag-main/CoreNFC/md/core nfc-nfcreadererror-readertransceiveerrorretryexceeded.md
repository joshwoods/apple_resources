

- Core NFC
- NFCReaderError
-  readerTransceiveErrorRetryExceeded 

Type Property

# readerTransceiveErrorRetryExceeded

Too many retries have occurred.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
static var readerTransceiveErrorRetryExceeded: NFCReaderError.Code { get }
```

## See Also

### Transceive Errors

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

