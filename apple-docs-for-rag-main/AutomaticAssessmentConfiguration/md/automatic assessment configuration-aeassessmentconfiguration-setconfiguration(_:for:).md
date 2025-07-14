

- Automatic Assessment Configuration
- AEAssessmentConfiguration
-  setConfiguration(\_:for:) 

Instance Method

# setConfiguration(\_:for:)

Adds an app to the list of apps available during an assessment.

iOS 17.5+iPadOS 17.5+Mac Catalyst 15.0+macOS 12.0+

``` source
func setConfiguration(
    _ configuration: AEAssessmentParticipantConfiguration,
    for application: AEAssessmentApplication
)
```

## Parameters 

`configuration`  

The configuration of the secondary app.

`application`  

The app that you want to configure.

## Discussion

Use this method to make an app besides your own available during an assessment. Create a representation of the app that you want to allow as an AEAssessmentApplication instance, and the configuration for that app using an AEAssessmentParticipantConfiguration instance:

```
let calculator = AEAssessmentApplication(bundleIdentifier: "com.apple.calculator")
let calculatorConfig = AEAssessmentParticipantConfiguration()
calculatorConfig.allowsNetworkAccess = false // Calculator doesn't need the network.
```

Use the app and its configuration to create an assessment configuration, and either create an assessment session with that, or update an existing session as shown below:

```
let configuration = AEAssessmentConfiguration()
configuration.setConfiguration(calculatorConfig, for: calculator)
session.update(to: configuration)
```

You can get a list of the currently allowed apps by accessing the configurationsByApplication property. You can disallow a previously allowed app by using the remove(_:) method.

## See Also

### Allowing access to other apps

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

