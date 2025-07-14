

- Contacts
-  CNChangeHistoryEventVisitor 

Protocol

# CNChangeHistoryEventVisitor

An interface for receiving notice of changes to contacts and groups.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
protocol CNChangeHistoryEventVisitor : NSObjectProtocol
```

## Overview

Implement this protocol to receive events that describe when a user adds, updates, or deletes contacts or groups outside your app.

## Topics

### Updating contacts

func visit(CNChangeHistoryAddContactEvent)

Tells the delegate that the user added a contact.

**Required**

func visit(CNChangeHistoryUpdateContactEvent)

Tells the delegate that the user updated a contact.

**Required**

func visit(CNChangeHistoryDeleteContactEvent)

Tells the delegate that the user deleted a contact.

**Required**

### Updating groups

func visit(CNChangeHistoryAddGroupEvent)

Tells the delegate that the user added a group.

func visit(CNChangeHistoryUpdateGroupEvent)

Tells the delegate that the user updated a group.

func visit(CNChangeHistoryDeleteGroupEvent)

Tells the delegate that the user deleted a group.

### Updating subgroups

func visitAddSubgroup(CNChangeHistoryAddSubgroupToGroupEvent)

Tells the delegate that the user added a subgroup to a group.

func visitRemoveSubgroup(CNChangeHistoryRemoveSubgroupFromGroupEvent)

Tells the delegate that the user removed a subgroup from a group.

### Updating contacts in groups

func visitAddMember(CNChangeHistoryAddMemberToGroupEvent)

Tells the delegate that the user added a contact to a group.

func visitRemoveMember(CNChangeHistoryRemoveMemberFromGroupEvent)

Tells the delegate that the user removed a contact from a group.

### Resetting synced data

func visit(CNChangeHistoryDropEverythingEvent)

Tells the delegate to drop all contacts and groups before handling more events.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

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

class CNChangeHistoryRemoveMemberFromGroupEvent

An object that represents a user removing a contact from a group.

class CNChangeHistoryRemoveSubgroupFromGroupEvent

An object that represents a user removing a subgroup from a group.

class CNChangeHistoryUpdateContactEvent

An object that represents a user updating a contact.

class CNChangeHistoryUpdateGroupEvent

An object that represents an updated group event.

