

- Automatic Assessment Configuration
- AEAssessmentConfiguration
-  allowsKeyboardShortcuts 

Instance Property

# allowsKeyboardShortcuts

A Boolean value that indicates whether to allow keyboard shortcuts during an assessment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var allowsKeyboardShortcuts: Bool { get set }
```

## Discussion

Users can add Keyboard Shortcuts in the Settings app (General \> Keyboard \> Text Replacement). An assessment session disables the use of keyboard shortcuts by default, but you can allow them by setting allowsKeyboardShortcuts to `true` in the AEAssessmentConfiguration instance that you use to initialize a session.

## See Also

### Allowing typing assistance

var allowsContinuousPathKeyboard: Bool

A Boolean value that indicates whether to allow Slide to Type to operate during an assessment.

var allowsPredictiveKeyboard: Bool

A Boolean value that indicates whether to enable the predictive keyboard during an assessment.

var allowsPasswordAutoFill: Bool

A Boolean value that indicates whether to allow password autofill during an assessment.

