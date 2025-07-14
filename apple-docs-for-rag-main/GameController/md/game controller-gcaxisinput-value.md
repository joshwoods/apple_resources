

- Game Controller
- GCAxisInput
-  value 

Instance Property

# value

The value along the axis, in unit coordinates.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var value: Float { get }
```

**Required**

## See Also

### Getting the value

var valueDidChangeHandler: ((any GCPhysicalInputElement, any GCAxisInput, Float) -> Void)?

The block that the input object calls when the value changes.

**Required**

var lastValueTimestamp: TimeInterval

The time of the most recent value change.

**Required**

var lastValueLatency: TimeInterval

The time in seconds between the last value change and the current time.

**Required**

