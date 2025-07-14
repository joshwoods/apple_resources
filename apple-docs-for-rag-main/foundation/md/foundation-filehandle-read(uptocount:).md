

- Foundation
- FileHandle
-  read(upToCount:) 

Instance Method

# read(upToCount:)

Reads data synchronously up to the specified number of bytes.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+tvOS 13.4+visionOS 1.0+watchOS 6.2+

``` source
func read(upToCount count: Int) throws -> Data?
```

## Parameters 

`count`  

The number of bytes to read from the file handle.

## Return Value

The data available through the receiver up to a maximum of `length` bytes, or the maximum size that can be represented by an NSData object, whichever is the smaller.

## Discussion

If the handle represents a file, this method returns the data obtained by reading `length` bytes starting at the current file pointer. If `length` bytes aren’t available, this method returns the data from the current file pointer to the end of the file. If the handle is a communications channel, the method reads up to `length` bytes from the channel. Returns an empty NSData object if the handle is at the file’s end or if the communications channel returns an end-of-file indicator.

This method throws an error if attempts to determine the file-handle type fail or if attempts to read from the file or channel fail.

## See Also

### Reading from a File Handle Synchronously

var availableData: Data

The data currently available in the receiver.

func readToEnd() throws -> Data?

Reads the available data synchronously up to the end of file or maximum number of bytes.

