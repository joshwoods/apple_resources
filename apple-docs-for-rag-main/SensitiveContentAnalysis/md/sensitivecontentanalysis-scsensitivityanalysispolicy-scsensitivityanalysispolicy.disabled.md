

- SensitiveContentAnalysis
- SCSensitivityAnalysisPolicy
-  SCSensitivityAnalysisPolicy.disabled 

Case

# SCSensitivityAnalysisPolicy.disabled

An indicator that the app lacks access to use the framework.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.0+

``` source
case disabled
```

## Mentioned in 

Detecting nudity in media and providing intervention options

## Discussion

If analysisPolicy is this value, the framework doesn’t detect nudity. The system disables sensitive content analysis under any of the following conditions:

- The app lacks the necessary com.apple.developer.sensitivecontentanalysis.client entitlement.

- Neither the Sensitive Content Warning user preference nor the Communication Safety parental control in Screen Time are active.

- The user disables the Sensitive Content Warnings toggle in your app’s Settings.

## See Also

### Checking and intervention strategies

case simpleInterventions

An indicator that user preference requests discrete detection of sensitive content.

case descriptiveInterventions

An indicator that user preference requests overt detection of sensitive content.

