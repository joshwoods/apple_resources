

- Contacts
-  CNChangeHistoryRemoveMemberFromGroupEvent 

Class

# CNChangeHistoryRemoveMemberFromGroupEvent

An object that represents a user removing a contact from a group.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
class CNChangeHistoryRemoveMemberFromGroupEvent
```

## Topics

### Getting event details

var group: CNGroup

The group where the user removed a contact.

var member: CNContact

The contact that the user removed from the group.

## Relationships

### Inherits From

- CNChangeHistoryEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Change history data

class CNChangeHistoryAddContactEvent

An object that represents a user adding a contact.

class CNChangeHistoryAddGroupEvent

An object that represents a user adding a group.

class CNChangeHistoryAddMemberToGroupEvent

An object that represents a user adding a contact to a group.

class CNChangeHistoryAddSubgroupToGroupEvent

An object that represents a user adding a subgroup to a group.

class CNChangeHistoryDeleteContactEvent

An object that represents a user deleting a contact.

class CNChangeHistoryDeleteGroupEvent

An object that represents a user deleting a group.

class CNChangeHistoryDropEverythingEvent

An object that indicates the delegate should drop all contacts and groups before handling change events.

class CNChangeHistoryEvent

An object that represents the user adding, updating, or deleting a contact or group.

class CNChangeHistoryFetchRequest

An object that specifies the criteria for fetching change history.

class CNChangeHistoryRemoveSubgroupFromGroupEvent

An object that represents a user removing a subgroup from a group.

class CNChangeHistoryUpdateContactEvent

An object that represents a user updating a contact.

class CNChangeHistoryUpdateGroupEvent

An object that represents an updated group event.

protocol CNChangeHistoryEventVisitor

An interface for receiving notice of changes to contacts and groups.

