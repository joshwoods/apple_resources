

- Automatic Assessment Configuration
- AEAssessmentSessionDelegate
-  assessmentSessionDidBegin(\_:) 

Instance Method

# assessmentSessionDidBegin(\_:)

Tells the delegate that the session started.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15.4+

``` source
optional func assessmentSessionDidBegin(_ session: AEAssessmentSession)
```

## Parameters 

`session`  

The session that started.

## Discussion

After your app calls a session’s begin() method, the session asynchronously disables the appropriate system services and then calls its delegate’s assessmentSessionDidBegin(_:) method. Only after receiving this callback can you be sure that it’s safe to start an assessment. If the session fails to start for any reason, you receive a call to the assessmentSession(_:failedToBeginWithError:) method instead.

## See Also

### Responding to session start and stop

func assessmentSession(AEAssessmentSession, failedToBeginWithError: any Error)

Tells the delegate that the session failed to start.

func assessmentSession(AEAssessmentSession, wasInterruptedWithError: any Error)

Tells the delegate that a system failure interrupted the session.

func assessmentSessionDidEnd(AEAssessmentSession)

Tells the delegate that the session ended.

