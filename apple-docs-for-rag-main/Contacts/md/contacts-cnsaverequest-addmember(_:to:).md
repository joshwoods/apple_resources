

- Contacts
- CNSaveRequest
-  addMember(\_:to:) 

Instance Method

# addMember(\_:to:)

Adds a contact as a member of a group.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func addMember(
    _ contact: CNContact,
    to group: CNGroup
)
```

## Parameters 

`contact`  

The contact to add to the group membership.

`group`  

The group to add the contact to its membership.

## Discussion

This method overrides any previously made remove membership request on the contact from the group.

## See Also

### Saving group changes

func add(CNMutableGroup, toContainerWithIdentifier: String?)

Adds a group to the contact store.

func update(CNMutableGroup)

Updates an existing group in the contact store.

func delete(CNMutableGroup)

Deletes a group from the contact store.

func removeMember(CNContact, from: CNGroup)

Removes a contact as a member of a group.

