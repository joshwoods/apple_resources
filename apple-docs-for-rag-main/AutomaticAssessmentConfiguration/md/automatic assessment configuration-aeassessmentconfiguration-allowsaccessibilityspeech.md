

- Automatic Assessment Configuration
- AEAssessmentConfiguration
-  allowsAccessibilitySpeech 

Instance Property

# allowsAccessibilitySpeech

A Boolean value that indicates whether to allow the speech-related accessibility features during an assessment.

iOS 14.0+iPadOS 14.0+

``` source
var allowsAccessibilitySpeech: Bool { get set }
```

## Discussion

A device reads text aloud for users who need it. In particular, users can enable the following features from Accessibility \> Spoken Content in the Settings app on iOS and iPadOS:

- Speak Selection

- Speak Screen

- Typing Feedback \> Speak Words

An assessment session disables these features by default, but you can allow them by setting allowsAccessibilitySpeech to `true` in the AEAssessmentConfiguration instance that you use to initialize a session.

## See Also

### Allowing accessibility

var allowsDictation: Bool

A Boolean value that indicates whether to allow the use of dictation during an assessment.

