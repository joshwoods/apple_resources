

- Core NFC
- NFCReaderError
-  readerTransceiveErrorTagNotConnected 

Type Property

# readerTransceiveErrorTagNotConnected

The tag isn’t in the connected state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
static var readerTransceiveErrorTagNotConnected: NFCReaderError.Code { get }
```

## See Also

### Transceive Errors

static var readerTransceiveErrorRetryExceeded: NFCReaderError.Code

Too many retries have occurred.

static var readerTransceiveErrorTagConnectionLost: NFCReaderError.Code

The reader lost the connection to the tag.

static var readerTransceiveErrorTagResponseError: NFCReaderError.Code

The tag has responded with an error.

static var readerTransceiveErrorSessionInvalidated: NFCReaderError.Code

The reader session is invalid.

static var readerTransceiveErrorPacketTooLong: NFCReaderError.Code

The packet length exceeds the limit supported by the tag.

