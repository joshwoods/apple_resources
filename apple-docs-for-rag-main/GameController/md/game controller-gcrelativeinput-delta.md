

- Game Controller
- GCRelativeInput
-  delta 

Instance Property

# delta

The most recent amount of change in values that the profile records.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var delta: Float { get }
```

**Required**

## See Also

### Getting the delta value and timestamp

var deltaDidChangeHandler: ((any GCPhysicalInputElement, any GCRelativeInput, Float) -> Void)?

The block that the profile calls when the element’s input changes.

**Required**

var lastDeltaTimestamp: TimeInterval

A timestamp for when the profile reports the delta value.

**Required**

var lastDeltaLatency: TimeInterval

The time in seconds between the current and the previous delta values.

**Required**

