

- Automatic Assessment Configuration
- AEAssessmentConfiguration
-  allowsContinuousPathKeyboard 

Instance Property

# allowsContinuousPathKeyboard

A Boolean value that indicates whether to allow Slide to Type to operate during an assessment.

iOS 14.0+iPadOS 14.0+

``` source
var allowsContinuousPathKeyboard: Bool { get set }
```

## Discussion

Users can turn on Slide to Type in the Settings app (General \> Keyboard). An assessment session disables this feature by default, but you can allow it by setting allowsContinuousPathKeyboard to `true` in the AEAssessmentConfiguration instance that you use to initialize a session.

## See Also

### Allowing typing assistance

var allowsKeyboardShortcuts: Bool

A Boolean value that indicates whether to allow keyboard shortcuts during an assessment.

var allowsPredictiveKeyboard: Bool

A Boolean value that indicates whether to enable the predictive keyboard during an assessment.

var allowsPasswordAutoFill: Bool

A Boolean value that indicates whether to allow password autofill during an assessment.

