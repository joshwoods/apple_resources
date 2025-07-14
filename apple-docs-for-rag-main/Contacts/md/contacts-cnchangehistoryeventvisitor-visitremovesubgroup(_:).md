

- Contacts
- CNChangeHistoryEventVisitor
-  visitRemoveSubgroup(\_:) 

Instance Method

# visitRemoveSubgroup(\_:)

Tells the delegate that the user removed a subgroup from a group.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
optional func visitRemoveSubgroup(_ event: CNChangeHistoryRemoveSubgroupFromGroupEvent)
```

## Parameters 

`event`  

The event object that represents a user removing a subgroup from a group.

## Discussion

Inspect the group and subgroup in the event that the system provides and update your app’s cached data accordingly.

## See Also

### Updating subgroups

func visitAddSubgroup(CNChangeHistoryAddSubgroupToGroupEvent)

Tells the delegate that the user added a subgroup to a group.

