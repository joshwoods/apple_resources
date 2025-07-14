

- Foundation
- FileHandle
-  write(contentsOf:) 

Instance Method

# write(contentsOf:)

Writes the specified data synchronously to the file handle.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+tvOS 13.4+visionOS 1.0+watchOS 6.2+

``` source
func write(contentsOf data: T) throws where T : DataProtocol
```

## Parameters 

`data`  

The data to write to the file handle.

## Discussion

If the handle represents a file, writing takes place at the file pointer’s current position. After it writes the data, the method advances the file pointer by the number of bytes written. This method throws an error if the file descriptor is closed or isn’t valid, if the handle represents an unconnected pipe or socket endpoint, if there isn’t any free space on the file system, or if any other writing error occurs.

## See Also

### Related Documentation

var availableData: Data

The data currently available in the receiver.

func read(upToCount: Int) throws -> Data?

Reads data synchronously up to the specified number of bytes.

func readToEnd() throws -> Data?

Reads the available data synchronously up to the end of file or maximum number of bytes.

