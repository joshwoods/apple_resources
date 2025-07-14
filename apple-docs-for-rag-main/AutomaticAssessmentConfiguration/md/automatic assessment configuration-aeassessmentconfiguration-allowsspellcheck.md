

- Automatic Assessment Configuration
- AEAssessmentConfiguration
-  allowsSpellCheck 

Instance Property

# allowsSpellCheck

A Boolean value that indicates whether to allow spell check during an assessment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var allowsSpellCheck: Bool { get set }
```

## Discussion

Users can activate the spell checker by turning on the Check Spelling feature in the Settings app (General \> Keyboard). An assessment session disables spell checking by default, but you can allow it by setting allowsSpellCheck to `true` in the AEAssessmentConfiguration instance that you use to initialize a session.

## See Also

### Allowing corrections

var autocorrectMode: AEAssessmentConfiguration.AutocorrectMode

A Boolean value that indicates whether to allow Autocorrect during an assessment.

struct AutocorrectMode

The set of autocorrect features that you can enable during an assessment.

