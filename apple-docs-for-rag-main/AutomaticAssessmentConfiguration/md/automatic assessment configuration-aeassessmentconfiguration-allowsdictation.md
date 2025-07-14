

- Automatic Assessment Configuration
- AEAssessmentConfiguration
-  allowsDictation 

Instance Property

# allowsDictation

A Boolean value that indicates whether to allow the use of dictation during an assessment.

iOS 14.0+iPadOS 14.0+

``` source
var allowsDictation: Bool { get set }
```

## Discussion

By turning on Enable Dictation (General \> Keyboard in the Settings app on iOS and iPadOS), users can speak into their device and have the words they speak converted to text. An assessment session disables this feature by default, but you can allow it by setting allowsDictation to `true` in the AEAssessmentConfiguration instance that you use to initialize a session.

## See Also

### Allowing accessibility

var allowsAccessibilitySpeech: Bool

A Boolean value that indicates whether to allow the speech-related accessibility features during an assessment.

