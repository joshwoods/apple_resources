

- Automatic Assessment Configuration
- AEAssessmentConfiguration
-  allowsPasswordAutoFill 

Instance Property

# allowsPasswordAutoFill

A Boolean value that indicates whether to allow password autofill during an assessment.

iOS 14.0+iPadOS 14.0+

``` source
var allowsPasswordAutoFill: Bool { get set }
```

## Discussion

Users can store passwords for use with Password Autofill by turning on the feature in the Settings app (General \> Passwords \> AutoFill Passwords). An assessment session disables Password Autofill by default, but you can allow it by setting allowsPasswordAutoFill to `true` in the AEAssessmentConfiguration instance that you use to initialize a session.

## See Also

### Allowing typing assistance

var allowsContinuousPathKeyboard: Bool

A Boolean value that indicates whether to allow Slide to Type to operate during an assessment.

var allowsKeyboardShortcuts: Bool

A Boolean value that indicates whether to allow keyboard shortcuts during an assessment.

var allowsPredictiveKeyboard: Bool

A Boolean value that indicates whether to enable the predictive keyboard during an assessment.

