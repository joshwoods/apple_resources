

- Contacts
- CNChangeHistoryEventVisitor
-  visit(\_:) 

Instance Method

# visit(\_:)

Tells the delegate that the user deleted a group.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
optional func visit(_ event: CNChangeHistoryDeleteGroupEvent)
```

## Parameters 

`event`  

The event object that represents a user deleting a group.

## Discussion

Inspect the group identifier in the event that the system provides and update your app’s cached data accordingly.

## See Also

### Updating groups

func visit(CNChangeHistoryAddGroupEvent)

Tells the delegate that the user added a group.

func visit(CNChangeHistoryUpdateGroupEvent)

Tells the delegate that the user updated a group.

