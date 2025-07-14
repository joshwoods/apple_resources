

- UIKit
- UIPress
-  timestamp 

Instance Property

# timestamp

The time when the press occurred or when it was last mutated.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
var timestamp: TimeInterval { get }
```

## Discussion

The value of this property is the time, in seconds, from system startup to the time in which the touch either originated or was last changed. You can store and compare the initial value of this attribute to subsequent timestamp values of a UIPress instance to determine the duration of the press and, if it’s being swiped, the speed of movement. For a definition of the time-since-boot value, see the description of the ProcessInfo class’s systemUptime method.

## See Also

### Getting press attributes

var key: UIKey?

The key pressed or released on a physical keyboard.

var type: UIPress.PressType

The type of the specified press.

var phase: UIPress.Phase

The current press phase of the object.

