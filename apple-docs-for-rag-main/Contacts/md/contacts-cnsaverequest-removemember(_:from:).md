

- Contacts
- CNSaveRequest
-  removeMember(\_:from:) 

Instance Method

# removeMember(\_:from:)

Removes a contact as a member of a group.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func removeMember(
    _ contact: CNContact,
    from group: CNGroup
)
```

## Parameters 

`contact`  

The contact to remove from the group membership.

`group`  

The group to remove the contact from its membership.

## Discussion

This method removes the contact from the group, but does not delete it from the contact store. This method overrides any previously made add membership request on the contact to the group.

## See Also

### Saving group changes

func add(CNMutableGroup, toContainerWithIdentifier: String?)

Adds a group to the contact store.

func update(CNMutableGroup)

Updates an existing group in the contact store.

func delete(CNMutableGroup)

Deletes a group from the contact store.

func addMember(CNContact, to: CNGroup)

Adds a contact as a member of a group.

