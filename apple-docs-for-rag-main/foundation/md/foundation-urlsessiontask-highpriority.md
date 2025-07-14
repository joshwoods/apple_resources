

- Foundation
- URLSessionTask
-  highPriority 

Type Property

# highPriority

A high URL session task priority, with a floating point value above the default value and below the maximum of `1.0`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class let highPriority: Float
```

## See Also

### Priority constants

class let defaultPriority: Float

The default URL session task priority, used implicitly for any task you have not prioritized.

class let lowPriority: Float

A low URL session task priority, with a floating point value above the minimum of `0` and below the default value.

