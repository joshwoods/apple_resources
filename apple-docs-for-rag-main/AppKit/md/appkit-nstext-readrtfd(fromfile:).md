

- AppKit
- NSText
-  readRTFD(fromFile:) 

Instance Method

# readRTFD(fromFile:)

Attempts to read the RTFD file at `path`, returning true if successful and false if not.

macOS

``` source
@MainActor
func readRTFD(fromFile path: String) -> Bool
```

## Discussion

`path` should be the path for an `.rtf` file or an `.rtfd` file wrapper, not for the RTF file within an `.rtfd` file wrapper.

## See Also

### Reading and writing RTF files

func writeRTFD(toFile: String, atomically: Bool) -> Bool

Writes the receiver’s text as RTF with attachments to a file or directory at `path`.

func rtfd(from: NSRange) -> Data?

Returns an NSData object that contains an RTFD stream corresponding to the characters and attributes within `aRange`.

func rtf(from: NSRange) -> Data?

Returns an NSData object that contains an RTF stream corresponding to the characters and attributes within `aRange`, omitting any attachment characters and attributes.

