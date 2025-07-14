

- Core NFC
- NFCReaderError
-  ndefReaderSessionErrorTagSizeTooSmall 

Type Property

# ndefReaderSessionErrorTagSizeTooSmall

The NDEF tag memory size is too small to store the data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
static var ndefReaderSessionErrorTagSizeTooSmall: NFCReaderError.Code { get }
```

## See Also

### NDEF Tag Errors

static var ndefReaderSessionErrorTagNotWritable: NFCReaderError.Code

The NDEF tag isn’t writable.

static var ndefReaderSessionErrorTagUpdateFailure: NFCReaderError.Code

The reader session failed to update the NDEF tag.

static var ndefReaderSessionErrorZeroLengthMessage: NFCReaderError.Code

The NDEF tag doesn’t contain an NDEF message.

