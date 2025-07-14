

- Game Controller
- GCLinearInput
-  lastValueTimestamp 

Instance Property

# lastValueTimestamp

The time of the most recent value change.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var lastValueTimestamp: TimeInterval { get }
```

**Required**

## Discussion

This property isn’t a specific date and time. To determine the time between value changes, subtract a previous time from the current time.

## See Also

### Getting the value

var value: Float

The value in unit coordinates.

**Required**

var valueDidChangeHandler: ((any GCPhysicalInputElement, any GCLinearInput, Float) -> Void)?

The block that the profile calls when an element’s value changes.

**Required**

var lastValueLatency: TimeInterval

The time in seconds between the last value change and the current time.

**Required**

