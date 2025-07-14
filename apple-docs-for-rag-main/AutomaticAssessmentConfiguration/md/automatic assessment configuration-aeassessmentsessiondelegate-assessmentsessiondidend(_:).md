

- Automatic Assessment Configuration
- AEAssessmentSessionDelegate
-  assessmentSessionDidEnd(\_:) 

Instance Method

# assessmentSessionDidEnd(\_:)

Tells the delegate that the session ended.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15.4+

``` source
optional func assessmentSessionDidEnd(_ session: AEAssessmentSession)
```

## Parameters 

`session`  

The session that ended.

## Discussion

After your app calls a session’s end() method, the system asynchronously restores the system to its normal state and then calls its delegate’s assessmentSessionDidEnd(_:) method. Confirm to the user that the assessment has stopped only after receiving this callback.

## See Also

### Responding to session start and stop

func assessmentSessionDidBegin(AEAssessmentSession)

Tells the delegate that the session started.

func assessmentSession(AEAssessmentSession, failedToBeginWithError: any Error)

Tells the delegate that the session failed to start.

func assessmentSession(AEAssessmentSession, wasInterruptedWithError: any Error)

Tells the delegate that a system failure interrupted the session.

