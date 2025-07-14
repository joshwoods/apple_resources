

- CloudKit JS
-  CloudKit.ShareParticipantType 

Enumeration

# CloudKit.ShareParticipantType

Determines whether a participant can modify the list of participants of a shared record.

CloudKit JS 1.0+

``` source
interface CloudKit.ShareParticipantType {
 const String UNKNOWN;
 const String PRIVATE_USER;
 const String PUBLIC_USER;
 const String OWNER;
};
```

## Topics

### Enumeration Cases

OWNER

The owner of the shared record who can add private users but not add public users.

PRIVATE_USER

Participants who were invited to share the record by the owner.

PUBLIC_USER

Participants who accepted a shared record by accessing the share URL.

UNKNOWN

Unknown type of participant.

## See Also

### Enumerations

CloudKit.AppleIDButtonTheme

Specifies the look of the Apple ID button.

CloudKit.DatabaseScope

Available database scopes.

CloudKit.QueryFilterComparator

The comparators you use to create queries.

CloudKit.ReferenceAction

The delete action for a reference object.

CloudKit.ShareParticipantAcceptanceStatus

The status of a participant accepting a share invitation.

CloudKit.ShareParticipantPermission

The status of a participant accepting a share invitation.

CloudKit.SubscriptionType

The type of subscription.

