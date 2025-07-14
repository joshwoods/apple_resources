

- Automatic Assessment Configuration
- AEAssessmentConfiguration
-  allowsPredictiveKeyboard 

Instance Property

# allowsPredictiveKeyboard

A Boolean value that indicates whether to enable the predictive keyboard during an assessment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var allowsPredictiveKeyboard: Bool { get set }
```

## Discussion

Users can turn on the Predictive Keyboard feature in the Settings app (General \> Keyboard). An assessment session disables this feature by default, but you can allow it by setting allowsPredictiveKeyboard to `true` in the AEAssessmentConfiguration instance that you use to initialize a session.

## See Also

### Allowing typing assistance

var allowsContinuousPathKeyboard: Bool

A Boolean value that indicates whether to allow Slide to Type to operate during an assessment.

var allowsKeyboardShortcuts: Bool

A Boolean value that indicates whether to allow keyboard shortcuts during an assessment.

var allowsPasswordAutoFill: Bool

A Boolean value that indicates whether to allow password autofill during an assessment.

