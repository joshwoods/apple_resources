

- Game Controller
- GCPhysicalInputProfile
-  lastEventTimestamp 

Instance Property

# lastEventTimestamp

The time of the most recent change to an element’s value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var lastEventTimestamp: TimeInterval { get }
```

## See Also

### Getting change information

var valueDidChangeHandler: ((GCPhysicalInputProfile, GCControllerElement) -> Void)?

The block that the profile calls when an element’s value changes.

