

- Contacts
- CNChangeHistoryEventVisitor
-  visitRemoveMember(\_:) 

Instance Method

# visitRemoveMember(\_:)

Tells the delegate that the user removed a contact from a group.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
optional func visitRemoveMember(_ event: CNChangeHistoryRemoveMemberFromGroupEvent)
```

## Parameters 

`event`  

The event object that represents a user removing a contact from a group.

## Discussion

Inspect the group and contact in the event that the system provides and update your app’s cached data accordingly.

## See Also

### Updating contacts in groups

func visitAddMember(CNChangeHistoryAddMemberToGroupEvent)

Tells the delegate that the user added a contact to a group.

