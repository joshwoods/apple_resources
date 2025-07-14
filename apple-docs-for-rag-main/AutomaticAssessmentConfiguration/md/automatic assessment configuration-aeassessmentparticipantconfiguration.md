

- Automatic Assessment Configuration
-  AEAssessmentParticipantConfiguration 

Class

# AEAssessmentParticipantConfiguration

Configuration information for an app that’s available during an assessment.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AEAssessmentParticipantConfiguration
```

## Overview

Use an instance of this class to configure the properties of an app that you allow to run during an assessment. Associate the participant configuration with an app (an AEAssessmentApplication instance) when you call the setConfiguration(_:for:) method of a session configuration.

## Topics

### Creating participant configuration instances

init()

Initializes an assessment participant configuration instance.

class func new() -> Self

Creates a new assessment participant configuration instance.

### Allowing network access

var allowsNetworkAccess: Bool

A Boolean that indicates whether an app can access network resources during an assessment.

### Instance Properties

var configurationInfo: [String : Any]

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

class AEAssessmentApplication

A representation of an app that users can access during an assessment.

