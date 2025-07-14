

- Automatic Assessment Configuration
- AEAssessmentSessionDelegate
-  assessmentSessionDidUpdate(\_:) 

Instance Method

# assessmentSessionDidUpdate(\_:)

Tells the delegate that a configuration update succeeded.

iOS 17.5+iPadOS 17.5+Mac Catalyst 15.0+macOS 12.0+

``` source
optional func assessmentSessionDidUpdate(_ session: AEAssessmentSession)
```

## Parameters 

`session`  

The session that received the configuration update.

## Discussion

After you call a session’s update(to:) method, the session calls this delegate method to indicate a successful update. If the update fails, the session calls assessmentSession(_:failedToUpdateTo:error:) instead.

## See Also

### Responding to configuration changes

func assessmentSession(AEAssessmentSession, failedToUpdateTo: AEAssessmentConfiguration, error: any Error)

Tells the delegate that a configuration update failed.

