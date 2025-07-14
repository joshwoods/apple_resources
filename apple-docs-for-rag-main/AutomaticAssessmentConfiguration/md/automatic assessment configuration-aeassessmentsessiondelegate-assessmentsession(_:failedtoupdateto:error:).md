

- Automatic Assessment Configuration
- AEAssessmentSessionDelegate
-  assessmentSession(\_:failedToUpdateTo:error:) 

Instance Method

# assessmentSession(\_:failedToUpdateTo:error:)

Tells the delegate that a configuration update failed.

iOS 17.5+iPadOS 17.5+Mac Catalyst 15.0+macOS 12.0+

``` source
optional func assessmentSession(
    _ session: AEAssessmentSession,
    failedToUpdateTo configuration: AEAssessmentConfiguration,
    error: any Error
)
```

## Parameters 

`session`  

The session that you attempted to update.

`configuration`  

The configuration that you attempted to update the session with.

`error`  

An error that describes the reason for the failure.

## Discussion

After you call a session’s update(to:) method, the session calls this delegate method if the update fails. If the update succeeds, the session calls assessmentSessionDidUpdate(_:) instead.

## See Also

### Responding to configuration changes

func assessmentSessionDidUpdate(AEAssessmentSession)

Tells the delegate that a configuration update succeeded.

