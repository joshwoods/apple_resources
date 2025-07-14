

- AppKit
- NSText
-  writeRTFD(toFile:atomically:) 

Instance Method

# writeRTFD(toFile:atomically:)

Writes the receiver’s text as RTF with attachments to a file or directory at `path`.

macOS

``` source
@MainActor
func writeRTFD(
    toFile path: String,
    atomically flag: Bool
) -> Bool
```

## Discussion

Returns true on success and false on failure. If `atomicFlag` is true, attempts to write the file safely so that an existing file at `path` is not overwritten, nor does a new file at `path` actually get created, unless the write is successful.

## See Also

### Reading and writing RTF files

func readRTFD(fromFile: String) -> Bool

Attempts to read the RTFD file at `path`, returning true if successful and false if not.

func rtfd(from: NSRange) -> Data?

Returns an NSData object that contains an RTFD stream corresponding to the characters and attributes within `aRange`.

func rtf(from: NSRange) -> Data?

Returns an NSData object that contains an RTF stream corresponding to the characters and attributes within `aRange`, omitting any attachment characters and attributes.

