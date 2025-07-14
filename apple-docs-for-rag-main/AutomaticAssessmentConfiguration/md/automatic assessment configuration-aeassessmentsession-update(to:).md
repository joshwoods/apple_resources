

- Automatic Assessment Configuration
- AEAssessmentSession
-  update(to:) 

Instance Method

# update(to:)

Changes the session to use the specified configuration.

iOS 17.5+iPadOS 17.5+Mac Catalyst 15.0+macOS 12.0+

``` source
func update(to configuration: AEAssessmentConfiguration)
```

## Parameters 

`configuration`  

A new configuration to use for the session.

## Discussion

After you call this method, the session tries to apply the new configuration and then calls its delegate’s assessmentSessionDidUpdate(_:) method to indicate success, or the delegate’s assessmentSession(_:failedToUpdateTo:error:) method to indicate failure. Wait to receive one of these callbacks before proceeding with an assessment, and be sure to handle the failure case.

## See Also

### Managing session configuration

var configuration: AEAssessmentConfiguration

The current configuration of the session.

class var supportsMultipleParticipants: Bool

A Boolean that indicates whether the current device or platform supports a configuration with one or more participant applications.

class var supportsConfigurationUpdates: Bool

A Boolean that indicates whether the current device or platform supports updating a session’s configuration after the session has begun.

