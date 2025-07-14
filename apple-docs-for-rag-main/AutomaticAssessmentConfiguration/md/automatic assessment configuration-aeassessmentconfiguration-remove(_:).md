

- Automatic Assessment Configuration
- AEAssessmentConfiguration
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the availability of a previously allowed app.

iOS 17.5+iPadOS 17.5+Mac Catalyst 15.0+macOS 12.0+

``` source
func remove(_ application: AEAssessmentApplication)
```

## Parameters 

`application`  

The app that you want to remove from the list of allowed secondary apps.

## Discussion

Use this method to remove apps that you previously added to the list of apps that are available during an assessment with the setConfiguration(_:for:) method. You can get the list of currently allowed apps by accessing the configuration’s configurationsByApplication property.

## See Also

### Allowing access to other apps

func setConfiguration(AEAssessmentParticipantConfiguration, for: AEAssessmentApplication)

Adds an app to the list of apps available during an assessment.

var configurationsByApplication: [AEAssessmentApplication : AEAssessmentParticipantConfiguration]

The collection of apps available during an assessment, along with their associated configurations.

var mainParticipantConfiguration: AEAssessmentParticipantConfiguration

The app-specific configuration for the app that invokes the assessment.

class AEAssessmentApplication

A representation of an app that users can access during an assessment.

class AEAssessmentParticipantConfiguration

Configuration information for an app that’s available during an assessment.

