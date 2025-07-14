

- Foundation
- FileHandle
-  synchronizeFile() Deprecated

Instance Method

# synchronizeFile()

Causes all in-memory data and attributes of the file represented by the handle to write to permanent storage.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func synchronizeFile()
```

Deprecated

Use synchronize() to handle errors when synchronizing the file.

## Discussion

Programs that require the file to always be in a known state should call this method. An invocation of this method doesn’t return until memory is flushed.

Important

This method raises fileHandleOperationException if called on a file handle representing a pipe or socket, if the file descriptor is closed, or if the operation failed.

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

func truncateFile(atOffset: UInt64)

Truncates or extends the file represented by the file handle to a specified offset within the file and puts the file pointer at that position.

Deprecated

let NSFileHandleNotificationMonitorModes: String

Currently unused.

Deprecated

