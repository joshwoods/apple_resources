

- Automatic Assessment Configuration
-  AEAssessmentApplication 

Class

# AEAssessmentApplication

A representation of an app that users can access during an assessment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AEAssessmentApplication
```

## Overview

Use an instance of this class when you want to make an app besides yours, like a calculator or a dictionary, available during an assessment. Create a representation of the app that you want to allow using the app’s bundle identifier and optionally the identifier of the team that distributes the app. You can get both identifiers for an app that you have installed using the `codesign` command line utility:

```
```

By default, the system requires that the app’s code signature is valid, and that either Apple distributes the app, or the developer notarizes the app or distributes it through the App Store. You can relax these requirements by setting the requiresSignatureValidation property to `false`, but that creates a potential security risk. In that case, the only requirement is that the app has the specified bundle and team identifiers. Prefer to keep the signature requirement.

Add the app to a session configuration by calling the setConfiguration(_:for:) method, and then apply the configuration to either a new session that you create, or an existing session with the update(to:) method.

## Topics

### Creating an assessment application

init(bundleIdentifier: String, teamIdentifier: String?)

Creates a representation of an app using its bundle and team identifiers.

init(bundleIdentifier: String)

Creates a representation of an app using its bundle identifier.

var bundleIdentifier: String

The bundle identifier of the app.

var teamIdentifier: String?

The team identifier of the app.

### Requiring code-signed apps

var requiresSignatureValidation: Bool

A Boolean that indicates whether the session requires the app to have a valid code signature to run.

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

### Allowing access to other apps

func setConfiguration(AEAssessmentParticipantConfiguration, for: AEAssessmentApplication)

Adds an app to the list of apps available during an assessment.

var configurationsByApplication: [AEAssessmentApplication : AEAssessmentParticipantConfiguration]

The collection of apps available during an assessment, along with their associated configurations.

func remove(AEAssessmentApplication)

Removes the availability of a previously allowed app.

var mainParticipantConfiguration: AEAssessmentParticipantConfiguration

The app-specific configuration for the app that invokes the assessment.

class AEAssessmentParticipantConfiguration

Configuration information for an app that’s available during an assessment.

