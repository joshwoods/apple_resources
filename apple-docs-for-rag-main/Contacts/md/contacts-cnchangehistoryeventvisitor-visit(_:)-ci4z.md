

- Contacts
- CNChangeHistoryEventVisitor
-  visit(\_:) 

Instance Method

# visit(\_:)

Tells the delegate that the user deleted a contact.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
func visit(_ event: CNChangeHistoryDeleteContactEvent)
```

**Required**

## Parameters 

`event`  

The event object that represents a user deleting a contact.

## Discussion

Inspect the contact identifier in the event that the system provides and update your app’s cached data accordingly.

## See Also

### Updating contacts

func visit(CNChangeHistoryAddContactEvent)

Tells the delegate that the user added a contact.

**Required**

func visit(CNChangeHistoryUpdateContactEvent)

Tells the delegate that the user updated a contact.

**Required**

