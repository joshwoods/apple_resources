

- Automatic Assessment Configuration
- AEAssessmentSessionDelegate
-  assessmentSession(\_:failedToBeginWithError:) 

Instance Method

# assessmentSession(\_:failedToBeginWithError:)

Tells the delegate that the session failed to start.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15.4+

``` source
optional func assessmentSession(
    _ session: AEAssessmentSession,
    failedToBeginWithError error: any Error
)
```

## Parameters 

`session`  

The session that failed to start.

`error`  

An error that provides information about why the session failed.

## Discussion

After your app calls a session’s begin() method, the session asynchronously disables the appropriate system services and then calls its delegate’s assessmentSessionDidBegin(_:) method. However, if the session fails to start for any reason, it calls the assessmentSession(_:failedToBeginWithError:) method instead. Don’t start any assessments if your app receives this callback.

## See Also

### Responding to session start and stop

func assessmentSessionDidBegin(AEAssessmentSession)

Tells the delegate that the session started.

func assessmentSession(AEAssessmentSession, wasInterruptedWithError: any Error)

Tells the delegate that a system failure interrupted the session.

func assessmentSessionDidEnd(AEAssessmentSession)

Tells the delegate that the session ended.

