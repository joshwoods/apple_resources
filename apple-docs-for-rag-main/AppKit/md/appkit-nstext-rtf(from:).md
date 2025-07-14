

- AppKit
- NSText
-  rtf(from:) 

Instance Method

# rtf(from:)

Returns an NSData object that contains an RTF stream corresponding to the characters and attributes within `aRange`, omitting any attachment characters and attributes.

macOS

``` source
@MainActor
func rtf(from range: NSRange) -> Data?
```

## Discussion

Raises an `NSRangeException` if any part of `aRange` lies beyond the end of the receiver’s characters.

When writing data to the pasteboard, you can use the NSData object as the first argument to `NSPasteboard`’s setData(_:forType:) method, with a second argument of `NSRTFPboardType`.

## See Also

### Reading and writing RTF files

func readRTFD(fromFile: String) -> Bool

Attempts to read the RTFD file at `path`, returning true if successful and false if not.

func writeRTFD(toFile: String, atomically: Bool) -> Bool

Writes the receiver’s text as RTF with attachments to a file or directory at `path`.

func rtfd(from: NSRange) -> Data?

Returns an NSData object that contains an RTFD stream corresponding to the characters and attributes within `aRange`.

