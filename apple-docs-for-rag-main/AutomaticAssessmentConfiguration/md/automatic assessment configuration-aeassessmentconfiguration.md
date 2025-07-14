

- Automatic Assessment Configuration
-  AEAssessmentConfiguration 

Class

# AEAssessmentConfiguration

Configuration information for an assessment session.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15.4+

``` source
class AEAssessmentConfiguration
```

## Overview

Create a configuration instance and pass it to the init(configuration:) initializer of an AEAssessmentSession instance to create a new assessment session. Before using the configuration, indicate which exceptions you want to allow for the assessment session’s restrictions by setting values on the configuration instance. For example, you can set values to allow dictation and certain aspects of autocorrect:

- Swift
- Objective-C

```
let config = AEAssessmentConfiguration()

#if os(iOS) // These exceptions available only on iOS and iPadOS.
config.allowsDictation = true
config.autocorrectMode = [.punctuation, .spelling]
#endif

let session = AEAssessmentSession(configuration: config)
```

```
AEAssessmentConfiguration *config = [AEAssessmentConfiguration new];

#if TARGET_OS_IPHONE || TARGET_IPHONE_SIMULATOR // These exceptions available only on iOS and iPadOS.
config.allowsDictation = YES;
config.autocorrectMode = AEAutocorrectModePunctuation | AEAutocorrectModeSpelling;
#endif

AEAssessmentSession *session = [[AEAssessmentSession alloc] initWithConfiguration:config];
```

While you provide a configuration instance when creating a session on iOS, iPadOS, and macOS, specific exceptions apply only to certain platforms. In particular, on macOS, you can selectively make specific apps besides your own available during an assessment — for example, to allow users to access a calculator or a dictionary. All other exceptions apply only to iOS and iPadOS.

## Topics

### Allowing access to other apps

func setConfiguration(AEAssessmentParticipantConfiguration, for: AEAssessmentApplication)

Adds an app to the list of apps available during an assessment.

var configurationsByApplication: [AEAssessmentApplication : AEAssessmentParticipantConfiguration]

The collection of apps available during an assessment, along with their associated configurations.

func remove(AEAssessmentApplication)

Removes the availability of a previously allowed app.

var mainParticipantConfiguration: AEAssessmentParticipantConfiguration

The app-specific configuration for the app that invokes the assessment.

class AEAssessmentApplication

A representation of an app that users can access during an assessment.

class AEAssessmentParticipantConfiguration

Configuration information for an app that’s available during an assessment.

### Allowing accessibility

var allowsAccessibilitySpeech: Bool

A Boolean value that indicates whether to allow the speech-related accessibility features during an assessment.

var allowsDictation: Bool

A Boolean value that indicates whether to allow the use of dictation during an assessment.

### Allowing typing assistance

var allowsContinuousPathKeyboard: Bool

A Boolean value that indicates whether to allow Slide to Type to operate during an assessment.

var allowsKeyboardShortcuts: Bool

A Boolean value that indicates whether to allow keyboard shortcuts during an assessment.

var allowsPredictiveKeyboard: Bool

A Boolean value that indicates whether to enable the predictive keyboard during an assessment.

var allowsPasswordAutoFill: Bool

A Boolean value that indicates whether to allow password autofill during an assessment.

### Allowing corrections

var allowsSpellCheck: Bool

A Boolean value that indicates whether to allow spell check during an assessment.

var autocorrectMode: AEAssessmentConfiguration.AutocorrectMode

A Boolean value that indicates whether to allow Autocorrect during an assessment.

struct AutocorrectMode

The set of autocorrect features that you can enable during an assessment.

### Allowing handoff

var allowsActivityContinuation: Bool

A Boolean value that indicates whether to allow Handoff during an assessment.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Sessions

Preparing an educational assessment app for distribution

Ensure your app maintains academic integrity by reviewing assessment practices and managing system capabilities.

Build an Educational Assessment App

Ensure the academic integrity of your assessment app by using Automatic Assessment Configuration.

class AEAssessmentSession

A session that your app uses to protect an assessment.

