

- Contacts
-  CNChangeHistoryDropEverythingEvent 

Class

# CNChangeHistoryDropEverythingEvent

An object that indicates the delegate should drop all contacts and groups before handling change events.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
class CNChangeHistoryDropEverythingEvent
```

## Overview

The system sends this event to your delegate when the system determines that enough has changed since the last time your app fetched the history changes that an incremental update is no longer possible. Following the drop-everything event, your app receives an add event for each contact and group currently in the database. This allows you to implement full syncs and incremental syncs using the same code.

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

class CNChangeHistoryEvent

An object that represents the user adding, updating, or deleting a contact or group.

class CNChangeHistoryFetchRequest

An object that specifies the criteria for fetching change history.

class CNChangeHistoryRemoveMemberFromGroupEvent

An object that represents a user removing a contact from a group.

class CNChangeHistoryRemoveSubgroupFromGroupEvent

An object that represents a user removing a subgroup from a group.

class CNChangeHistoryUpdateContactEvent

An object that represents a user updating a contact.

class CNChangeHistoryUpdateGroupEvent

An object that represents an updated group event.

protocol CNChangeHistoryEventVisitor

An interface for receiving notice of changes to contacts and groups.

