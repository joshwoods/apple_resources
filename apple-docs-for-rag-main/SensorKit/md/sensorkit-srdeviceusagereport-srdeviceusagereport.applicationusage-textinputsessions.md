

- SensorKit
- SRDeviceUsageReport
- SRDeviceUsageReport.ApplicationUsage
-  textInputSessions 

Instance Property

# textInputSessions

The text input session types that occur during application usage.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
var textInputSessions: [SRTextInputSession] { get }
```

## Discussion

This property contains the text and input sources the framework records as the user enters text in an app. A text-input session starts when the user raises a keyboard and ends when the keyboard dismisses. However, the framework combines a text-input session that contains fewer than 20 words with the subsequent text-input sessions until reaching a 20-word minimum. The framework separates input modes (inputModes) such that one input mode doesn’t combine with a text-input session of another mode (such as Spanish-Mexico).

## See Also

### Inspecting Text Input

class SRTextInputSession

The characters a user types for a particular keyboard.

