

- Automatic Assessment Configuration
- AEAssessmentConfiguration
-  mainParticipantConfiguration 

Instance Property

# mainParticipantConfiguration

The app-specific configuration for the app that invokes the assessment.

iOS 17.5+iPadOS 17.5+Mac Catalyst 15.0+macOS 12.0+

``` source
var mainParticipantConfiguration: AEAssessmentParticipantConfiguration { get }
```

## Discussion

Use this property to get and customize the app-specific configuration that’s applied to your own app. For example, you can set the allowsNetworkAccess property for your own app:

- Swift
- Objective-C

```
let config = AEAssessmentConfiguration()
config.mainParticipantConfiguration.allowsNetworkAccess = false
```

```
AEAssessmentConfiguration *config = [[AEAssessmentConfiguration alloc] init];
[config mainParticipantConfiguration].allowsNetworkAccess = NO;
```

## See Also

### Allowing access to other apps

func setConfiguration(AEAssessmentParticipantConfiguration, for: AEAssessmentApplication)

Adds an app to the list of apps available during an assessment.

var configurationsByApplication: [AEAssessmentApplication : AEAssessmentParticipantConfiguration]

The collection of apps available during an assessment, along with their associated configurations.

func remove(AEAssessmentApplication)

Removes the availability of a previously allowed app.

class AEAssessmentApplication

A representation of an app that users can access during an assessment.

class AEAssessmentParticipantConfiguration

Configuration information for an app that’s available during an assessment.

