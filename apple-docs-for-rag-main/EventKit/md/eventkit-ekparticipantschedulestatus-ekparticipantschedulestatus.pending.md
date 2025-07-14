

- EventKit
- EKParticipantScheduleStatus
-  EKParticipantScheduleStatus.pending 

Case

# EKParticipantScheduleStatus.pending

The invitation is in the process of being sent.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
case pending
```

## See Also

### Constants

case none

The invitation hasn’t been sent yet.

case sent

The invitation has been sent, but it’s unclear if it was successfully delivered.

case delivered

The invitation has been sent and successfully delivered.

case recipientNotRecognized

The invitation wasn’t delivered because the source doesn’t recognize the recipient.

case noPrivileges

The invitation wasn’t delivered because of insufficient privileges.

case deliveryFailed

The invitation wasn’t delivered due to a temporary failure.

case cannotDeliver

The invitation wasn’t delivered because the system is unsure of how to deliver it.

case recipientNotAllowed

The invitation wasn’t delivered because scheduling with the participant isn’t allowed.

