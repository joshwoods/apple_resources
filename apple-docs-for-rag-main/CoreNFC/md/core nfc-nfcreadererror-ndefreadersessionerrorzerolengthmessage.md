

- Core NFC
- NFCReaderError
-  ndefReaderSessionErrorZeroLengthMessage 

Type Property

# ndefReaderSessionErrorZeroLengthMessage

The NDEF tag doesn’t contain an NDEF message.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
static var ndefReaderSessionErrorZeroLengthMessage: NFCReaderError.Code { get }
```

## See Also

### NDEF Tag Errors

static var ndefReaderSessionErrorTagNotWritable: NFCReaderError.Code

The NDEF tag isn’t writable.

static var ndefReaderSessionErrorTagSizeTooSmall: NFCReaderError.Code

The NDEF tag memory size is too small to store the data.

static var ndefReaderSessionErrorTagUpdateFailure: NFCReaderError.Code

The reader session failed to update the NDEF tag.

