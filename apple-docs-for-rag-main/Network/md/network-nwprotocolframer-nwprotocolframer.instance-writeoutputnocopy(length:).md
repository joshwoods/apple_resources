

- Network
- NWProtocolFramer
- NWProtocolFramer.Instance
-  writeOutputNoCopy(length:) 

Instance Method

# writeOutputNoCopy(length:)

Sends a specific number of bytes from a message while inside your output handler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func writeOutputNoCopy(length: Int) throws
```

## See Also

### Writing Output

func parseOutput(minimumIncompleteLength: Int, maximumLength: Int, parse: (UnsafeMutableRawBufferPointer?, Bool) -> Int) -> Bool

Examines the content of output data while inside your output handler.

func writeOutput(data: Data)

Sends arbitrary output data from your protocol to the next protocol.

func passThroughOutput()

Indicates that your protocol no longer needs to handle output data.

