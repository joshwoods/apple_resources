

- Audio Toolbox
- AUParameter
-  setValue(\_:originator:atHostTime:eventType:) 

Instance Method

# setValue(\_:originator:atHostTime:eventType:)

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func setValue(
    _ value: AUValue,
    originator: AUParameterObserverToken?,
    atHostTime hostTime: UInt64,
    eventType: AUParameterAutomationEventType
)
```

## See Also

### Managing Parameter Values

var value: AUValue

The parameter’s current value.

func setValue(AUValue, originator: AUParameterObserverToken?)

Sets the parameter’s value, avoiding redundant notifications to the originator.

func setValue(AUValue, originator: AUParameterObserverToken?, atHostTime: UInt64)

Sets the parameter’s value, preserving the host time of the gesture that initiated the change.

func string(fromValue: UnsafePointer&lt;AUValue>?) -> String

Gets the string representation of a parameter value.

func value(from: String) -> AUValue

Converts a string into a parameter value.

