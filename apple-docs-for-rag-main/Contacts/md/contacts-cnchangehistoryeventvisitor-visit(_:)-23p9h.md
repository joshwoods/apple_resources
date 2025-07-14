

- Contacts
- CNChangeHistoryEventVisitor
-  visit(\_:) 

Instance Method

# visit(\_:)

Tells the delegate that the user updated a group.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
optional func visit(_ event: CNChangeHistoryUpdateGroupEvent)
```

## Parameters 

`event`  

The event object that represents a user updating a group.

## Discussion

Inspect the group in the event that the system provides and update your app’s cached data accordingly.

## See Also

### Updating groups

func visit(CNChangeHistoryAddGroupEvent)

Tells the delegate that the user added a group.

func visit(CNChangeHistoryDeleteGroupEvent)

Tells the delegate that the user deleted a group.

