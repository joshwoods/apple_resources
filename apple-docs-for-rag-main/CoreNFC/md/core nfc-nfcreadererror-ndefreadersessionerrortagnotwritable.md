

- Core NFC
- NFCReaderError
-  ndefReaderSessionErrorTagNotWritable 

Type Property

# ndefReaderSessionErrorTagNotWritable

The NDEF tag isn’t writable.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
static var ndefReaderSessionErrorTagNotWritable: NFCReaderError.Code { get }
```

## See Also

### NDEF Tag Errors

static var ndefReaderSessionErrorTagSizeTooSmall: NFCReaderError.Code

The NDEF tag memory size is too small to store the data.

static var ndefReaderSessionErrorTagUpdateFailure: NFCReaderError.Code

The reader session failed to update the NDEF tag.

static var ndefReaderSessionErrorZeroLengthMessage: NFCReaderError.Code

The NDEF tag doesn’t contain an NDEF message.

