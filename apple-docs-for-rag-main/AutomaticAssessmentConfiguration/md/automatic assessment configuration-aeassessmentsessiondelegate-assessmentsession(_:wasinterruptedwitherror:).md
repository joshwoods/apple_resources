

- Automatic Assessment Configuration
- AEAssessmentSessionDelegate
-  assessmentSession(\_:wasInterruptedWithError:) 

Instance Method

# assessmentSession(\_:wasInterruptedWithError:)

Tells the delegate that a system failure interrupted the session.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15.4+

``` source
optional func assessmentSession(
    _ session: AEAssessmentSession,
    wasInterruptedWithError error: any Error
)
```

## Parameters 

`session`  

The session that failed.

`error`  

An error that provides information about the interruption.

## Discussion

If one or more subsystems fail during a session, the session tells its delegate by calling the assessmentSession(_:wasInterruptedWithError:) method. If your app receives this callback, immediately stop the assessment, hide all sensitive content, and end the session. Because it might take time for your app to stop the assessment, the session relies on your app to call the end() method:

- Swift
- Objective-C

```
func assessmentSession(_ session: AEAssessmentSession, wasInterruptedWithError error: Error) {
    // Hide sensitive UI and optionally store assessment progress.

    // End the session.
    session.end()
}
```

```
- (void)assessmentSession:(AEAssessmentSession *)session wasInterruptedWithError:(NSError *)error {
    // Hide sensitive UI and optionally store assessment progress.

    // End the session.
    [session end];
}
```

## See Also

### Responding to session start and stop

func assessmentSessionDidBegin(AEAssessmentSession)

Tells the delegate that the session started.

func assessmentSession(AEAssessmentSession, failedToBeginWithError: any Error)

Tells the delegate that the session failed to start.

func assessmentSessionDidEnd(AEAssessmentSession)

Tells the delegate that the session ended.

