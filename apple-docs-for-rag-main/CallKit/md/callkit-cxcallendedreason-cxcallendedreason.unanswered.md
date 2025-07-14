

- CallKit
- CXCallEndedReason
-  CXCallEndedReason.unanswered 

Case

# CXCallEndedReason.unanswered

The call never started connecting and was never explicitly ended, such as when an outgoing or incoming call times out.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
case unanswered
```

## See Also

### Constants

case failed

An error occurred while attempting to service the call.

case remoteEnded

The remote party explicitly ended the call.

case answeredElsewhere

Another device answered the call.

case declinedElsewhere

Another device declined the call.

