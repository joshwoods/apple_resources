

- Contacts
- CNChangeHistoryEventVisitor
-  visitAddMember(\_:) 

Instance Method

# visitAddMember(\_:)

Tells the delegate that the user added a contact to a group.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
optional func visitAddMember(_ event: CNChangeHistoryAddMemberToGroupEvent)
```

## Parameters 

`event`  

The event object that represents a user adding a contact to a group.

## Discussion

Inspect the group and contact in the event that the system provides and update your app’s cached data accordingly.

## See Also

### Updating contacts in groups

func visitRemoveMember(CNChangeHistoryRemoveMemberFromGroupEvent)

Tells the delegate that the user removed a contact from a group.

