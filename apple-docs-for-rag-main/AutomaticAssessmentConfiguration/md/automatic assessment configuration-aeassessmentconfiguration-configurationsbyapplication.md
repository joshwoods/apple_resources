

- Automatic Assessment Configuration
- AEAssessmentConfiguration
-  configurationsByApplication 

Instance Property

# configurationsByApplication

The collection of apps available during an assessment, along with their associated configurations.

iOS 17.5+iPadOS 17.5+Mac Catalyst 15.0+macOS 12.0+

``` source
var configurationsByApplication: [AEAssessmentApplication : AEAssessmentParticipantConfiguration] { get }
```

## Discussion

Access this property to get a list of the currently allowed secondary apps and their individual configurations. Add apps to the list by calling the setConfiguration(_:for:) method. Remove them from the list by calling the remove(_:) method.

## See Also

### Allowing access to other apps

func setConfiguration(AEAssessmentParticipantConfiguration, for: AEAssessmentApplication)

Adds an app to the list of apps available during an assessment.

func remove(AEAssessmentApplication)

Removes the availability of a previously allowed app.

var mainParticipantConfiguration: AEAssessmentParticipantConfiguration

The app-specific configuration for the app that invokes the assessment.

class AEAssessmentApplication

A representation of an app that users can access during an assessment.

class AEAssessmentParticipantConfiguration

Configuration information for an app that’s available during an assessment.

