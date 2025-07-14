

- os
-  maxOSLogArgumentCount 

Global Variable

# maxOSLogArgumentCount

The maximum number of interpolated expressions that a log message may contain.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
var maxOSLogArgumentCount: UInt8 { get }
```

## Discussion

For log messages that include interpolated values, the system imposes a limit on the total number of expressions that a single message may include. The following example shows a string that contains an interpolated value:

```
let fileID = 941
let message = "Created a file with ID \(fileID)"
```

## See Also

### Getting the Message Details

var bufferSize: Int

The byte size of the buffer that the logging system receives.

let interpolation: OSLogInterpolation

The log message’s string interpolation.

