

- Automatic Assessment Configuration
- AEAssessmentConfiguration
-  AEAssessmentConfiguration.AutocorrectMode 

Structure

# AEAssessmentConfiguration.AutocorrectMode

The set of autocorrect features that you can enable during an assessment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 18.0+macOS 15.0+

``` source
struct AutocorrectMode
```

## Overview

Use one or more of the autocorrect modes to set the autocorrectMode property of an AEAssessmentConfiguration instance. For example, you can enable both spelling and punctuation corrections by combining spelling and punctuation:

- Swift
- Objective-C

```
let config = AEAssessmentConfiguration()

#if os(iOS) // Available only on iOS and iPadOS.
config.autocorrectMode = [.punctuation, .spelling]
#endif

let session = AEAssessmentSession(configuration: config)
```

```
AEAssessmentConfiguration *config = [AEAssessmentConfiguration new];

#if TARGET_OS_IPHONE || TARGET_IPHONE_SIMULATOR // Available only on iOS and iPadOS.
config.autocorrectMode = AEAutocorrectModePunctuation | AEAutocorrectModeSpelling;
#endif

AEAssessmentSession *session = [[AEAssessmentSession alloc] initWithConfiguration:config];
```

## Topics

### Creating a mode

init(rawValue: UInt)

Creates a new mode instance.

### Modes

static var punctuation: AEAssessmentConfiguration.AutocorrectMode

A mode in which autocorrect checks punctuation as the user types.

static var spelling: AEAssessmentConfiguration.AutocorrectMode

A mode in which autocorrect checks for spelling as the user types.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Allowing corrections

var allowsSpellCheck: Bool

A Boolean value that indicates whether to allow spell check during an assessment.

var autocorrectMode: AEAssessmentConfiguration.AutocorrectMode

A Boolean value that indicates whether to allow Autocorrect during an assessment.

