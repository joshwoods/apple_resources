

- Automatic Assessment Configuration
- AEAssessmentSession
-  delegate 

Instance Property

# delegate

A delegate to which the session provides state change updates.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15.4+

``` source
weak var delegate: (any AEAssessmentSessionDelegate)? { get set }
```

## Discussion

An assessment session operates asynchronously because it takes time to make the changes associated with starting or stopping a session, and external events might affect the state of the session. Adopt the AEAssessmentSessionDelegate protocol to receive callbacks at key points in the session life cycle. Store your adopter in the session’s delegate property before starting a session.

By listening for delegate callbacks, you learn when you can safely start an assessment after calling the session’s begin() method, when the session has finished after calling the end() method, or if the session has been interrupted for some reason.

The session calls all delegate methods on the main thread.

## See Also

### Responding to session updates

protocol AEAssessmentSessionDelegate

An interface that the session uses to provide information about session state changes to a delegate.

