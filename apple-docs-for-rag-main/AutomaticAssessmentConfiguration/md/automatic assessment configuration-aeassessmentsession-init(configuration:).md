

- Automatic Assessment Configuration
- AEAssessmentSession
-  init(configuration:) 

Initializer

# init(configuration:)

Creates a new assessment session.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15.4+

``` source
init(configuration: AEAssessmentConfiguration)
```

## Parameters 

`configuration`  

Configuration information for the session.

## Discussion

After creating a new session, assign its delegate property before calling the begin() method to start a session. Wait for the delegate to receive the assessmentSessionDidBegin(_:) call before starting an assessment.

