

- Foundation
- FileHandle
-  readToEnd() 

Instance Method

# readToEnd()

Reads the available data synchronously up to the end of file or maximum number of bytes.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+tvOS 13.4+visionOS 1.0+watchOS 6.2+

``` source
func readToEnd() throws -> Data?
```

## Return Value

The data available through the file handle up to the maximum size that can be represented by an NSData object or, if a communications channel, until an end-of-file indicator is returned.

## Discussion

This method invokes readData(ofLength:) as part of its implementation.

## See Also

### Reading from a File Handle Synchronously

var availableData: Data

The data currently available in the receiver.

func read(upToCount: Int) throws -> Data?

Reads data synchronously up to the specified number of bytes.

