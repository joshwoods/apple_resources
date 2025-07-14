

- WatchKit
- WKInterfaceDevice
-  play(\_:) 

Instance Method

# play(\_:)

Gives haptic feedback to the user.

watchOS 2.0+

``` source
func play(_ type: WKHapticType)
```

## Parameters 

`type`  

The type of haptic feedback to play. Always use the defined haptic types for their intended purposes. For a list of possible values, see WKHapticType.

## Discussion

Use this method to engage the haptic engine in Apple Watch. The type of feedback you specify defines the specific feedback that is delivered.

This method has no effect when called while your shared WKExtension object’s applicationState property is either WKApplicationState.background or WKApplicationState.inactive. By default, you cannot play haptic feedback in the background. The only exception are apps with an active workout session. For more information, see Running workout sessions in HKWorkoutSession.

Do not call this method multiple times in quick succession. If the haptic engine is already engaged when you call this method, the system stops the current feedback and imposes a minimum delay of 100 milliseconds before engaging the engine to generate the new feedback. Use of the haptic engine also consumes power, and using the engine too much may create a noticeable drain on the Apple Watch battery, as well as a negative user experience.

Important

Do not call this method while gathering heart rate data using HealthKit. When you engage the haptic engine, HealthKit stops gathering heart rate data until after the haptic engine finishes.

## See Also

### Playing Haptic Feedback

enum WKHapticType

Constant indicating the style of feedback to deliver using haptics.

