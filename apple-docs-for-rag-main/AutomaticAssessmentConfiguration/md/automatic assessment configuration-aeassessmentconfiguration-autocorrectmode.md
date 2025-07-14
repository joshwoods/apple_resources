

- Automatic Assessment Configuration
- AEAssessmentConfiguration
-  autocorrectMode 

Instance Property

# autocorrectMode

A Boolean value that indicates whether to allow Autocorrect during an assessment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var autocorrectMode: AEAssessmentConfiguration.AutocorrectMode { get set }
```

## Discussion

Users can turn on autocorrect in the Settings app (General \> Keyboard \> Auto-Correction). An assessment session disables this feature by default, but you can allow it by setting autocorrectMode in the AEAssessmentConfiguration instance that you use to initialize a session. Set the mode’s value to some combination of the the values from the AEAssessmentConfiguration.AutocorrectMode structure.

## See Also

### Allowing corrections

var allowsSpellCheck: Bool

A Boolean value that indicates whether to allow spell check during an assessment.

struct AutocorrectMode

The set of autocorrect features that you can enable during an assessment.

