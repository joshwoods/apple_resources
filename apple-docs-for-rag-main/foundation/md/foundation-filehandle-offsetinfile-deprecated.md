

- Foundation
- FileHandle
-  offsetInFile Deprecated

Instance Property

# offsetInFile

The position of the file pointer within the file represented by the file handle.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
var offsetInFile: UInt64 { get }
```

Deprecated

To handle errors when getting the file pointer’s position, use offset() in Swift and getOffset:error: in Objective-C.

## Discussion

Raises fileHandleOperationException if called on a file handle representing a pipe or socket, or if the file descriptor is closed.

## See Also

### Deprecated

func readDataToEndOfFile() -> Data

Reads the available data synchronously up to the end of file or maximum number of bytes.

Deprecated

func readData(ofLength: Int) -> Data

Reads data synchronously up to the specified number of bytes.

Deprecated

func write(Data)

Writes the specified data synchronously to the file handle.

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

