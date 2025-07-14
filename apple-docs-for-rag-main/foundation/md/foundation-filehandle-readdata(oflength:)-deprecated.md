

- Foundation
- FileHandle
-  readData(ofLength:) Deprecated

Instance Method

# readData(ofLength:)

Reads data synchronously up to the specified number of bytes.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.0–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func readData(ofLength length: Int) -> Data
```

Deprecated

To handle errors when reading data from the file handle, use read(upToCount:) in Swift and readDataUpToLength:error: in Objective-C.

## Parameters 

`length`  

The number of bytes to read from the file handle.

## Return Value

The data available through the receiver up to a maximum of `length` bytes, or the maximum size that can be represented by an NSData object, whichever is the smaller.

## Discussion

If the handle represents a file, this method returns the data obtained by reading `length` bytes starting at the current file pointer. If `length` bytes aren’t available, this method returns the data from the current file pointer to the end of the file. If the handle represents a communications channel, the method reads up to `length` bytes from the channel. Returns an empty `NSData` object if the handle is at the file’s end or if the communications channel returns an end-of-file indicator.

Important

This method raises fileHandleOperationException if attempts to determine the file-handle type fail or if attempts to read from the file or channel fail.

## See Also

### Related Documentation

var availableData: Data

The data currently available in the receiver.

### Deprecated

func readDataToEndOfFile() -> Data

Reads the available data synchronously up to the end of file or maximum number of bytes.

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

