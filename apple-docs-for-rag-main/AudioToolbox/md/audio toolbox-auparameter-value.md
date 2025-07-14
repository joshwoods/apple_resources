

- Audio Toolbox
- AUParameter
-  value 

Instance Property

# value

The parameter’s current value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var value: AUValue { get set }
```

## See Also

### Managing Parameter Values

func setValue(AUValue, originator: AUParameterObserverToken?)

Sets the parameter’s value, avoiding redundant notifications to the originator.

func setValue(AUValue, originator: AUParameterObserverToken?, atHostTime: UInt64)

Sets the parameter’s value, preserving the host time of the gesture that initiated the change.

func setValue(AUValue, originator: AUParameterObserverToken?, atHostTime: UInt64, eventType: AUParameterAutomationEventType)

func string(fromValue: UnsafePointer&lt;AUValue>?) -> String

Gets the string representation of a parameter value.

func value(from: String) -> AUValue

Converts a string into a parameter value.

