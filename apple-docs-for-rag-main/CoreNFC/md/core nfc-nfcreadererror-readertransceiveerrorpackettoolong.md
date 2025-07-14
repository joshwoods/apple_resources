

- Core NFC
- NFCReaderError
-  readerTransceiveErrorPacketTooLong 

Type Property

# readerTransceiveErrorPacketTooLong

The packet length exceeds the limit supported by the tag.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static var readerTransceiveErrorPacketTooLong: NFCReaderError.Code { get }
```

## See Also

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

