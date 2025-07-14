

- SensitiveContentAnalysis
- SCSensitivityAnalysisPolicy
-  SCSensitivityAnalysisPolicy.simpleInterventions 

Case

# SCSensitivityAnalysisPolicy.simpleInterventions

An indicator that user preference requests discrete detection of sensitive content.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.0+

``` source
case simpleInterventions
```

## Mentioned in 

Detecting nudity in media and providing intervention options

## Discussion

If analysisPolicy is this value, it indicates that the user enables both of the following:

- Sensitive Content Warnings user preference

- Sensitive Content Warnings in your app’s settings

When your app detects nudity under this policy, your app needs to:

- Keep the intervention minimal by describing the issue briefly and updating your app’s UI unobstructively. For example, consider blurring and annotating the area that otherwise presents the sensitive content versus raising a new fullscreen alert.

- Intervene on the receipt of sensitve content over the network but allow the app to transmit content over the network unchecked.

## See Also

### Checking and intervention strategies

case disabled

An indicator that the app lacks access to use the framework.

case descriptiveInterventions

An indicator that user preference requests overt detection of sensitive content.

