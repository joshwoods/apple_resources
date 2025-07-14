

- SensitiveContentAnalysis
-  SCSensitivityAnalysisPolicy 

Enumeration

# SCSensitivityAnalysisPolicy

Configurations that represent the way the framework checks for sensitive content and how the app responds.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 2.0+

``` source
enum SCSensitivityAnalysisPolicy
```

## Overview

This enumeration defines the possible values for the SCSensitivityAnalyzer property analysisPolicy. The values of the policy determine how your app manages sensitive content detection.

```
// Check the current analysis policy. 
let policy = analyzer.analysisPolicy
if policy == .disabled { return } 
else if policy == .simpleInterventions {
    // The Sensitive Content Warning setting is active.
} else if policy == .descriptiveInterventions {
    // The Communication Safety setting is active.
}
```

For guidance about observing the active analysis policy, see Detecting nudity in media and providing intervention options.

## Topics

### Checking and intervention strategies

case disabled

An indicator that the app lacks access to use the framework.

case simpleInterventions

An indicator that user preference requests discrete detection of sensitive content.

case descriptiveInterventions

An indicator that user preference requests overt detection of sensitive content.

### Creating an analysis policy value

init?(rawValue: Int)

Creates an analysis policy value from the enumeration’s underlying type.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Content analysis

class SCSensitivityAnalyzer

An object that analyzes media for sensitive content.

