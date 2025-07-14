

- Foundation
- FileHandle
-  readDataToEndOfFile() Deprecated

Instance Method

# readDataToEndOfFile()

Reads the available data synchronously up to the end of file or maximum number of bytes.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func readDataToEndOfFile() -> Data
```

Deprecated

To handle errors when reading data from the file handle, use readToEnd() in Swift and readDataToEndOfFileAndReturnError: in Objective-C.

## Return Value

The data available through the receiver up to maximum size that can be represented by an NSData object or, if a communications channel, until an end-of-file indicator is returned.

## Discussion

This method invokes readData(ofLength:) as part of its implementation.

Important

This method raises fileHandleOperationException if attempts to determine the file-handle type fail or if attempts to read from the file or channel fail.

## See Also

### Related Documentation

var availableData: Data

The data currently available in the receiver.

### Deprecated

func readData(ofLength: Int) -> Data

Reads data synchronously up to the specified number of bytes.

Deprecated

func write(Data)

Writes the specified data synchronously to the file handle.

Deprecated

var offsetInFile: UInt64

The position of the file pointer within the file represented by the file handle.

Deprecated

func seekToEndOfFile() -> UInt64

Places the file pointer at the end of the file referenced by the file handle and returns the new file offset.

Deprecated

func seek(toFileOffset: UInt64)

Moves the file pointer to the specified offset within the file represented by the receiver.

Deprecated

func closeFile()

Disallows further access to the represented file or communications channel and signals end of file on communications channels that permit writing.

Deprecated

func synchronizeFile()

Causes all in-memory data and attributes of the file represented by the handle to write to permanent storage.

Deprecated

func truncateFile(atOffset: UInt64)

Truncates or extends the file represented by the file handle to a specified offset within the file and puts the file pointer at that position.

Deprecated

let NSFileHandleNotificationMonitorModes: String

Currently unused.

Deprecated

