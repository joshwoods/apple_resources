

- Contacts
- CNSaveRequest
-  add(\_:toContainerWithIdentifier:) 

Instance Method

# add(\_:toContainerWithIdentifier:)

Adds a group to the contact store.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func add(
    _ group: CNMutableGroup,
    toContainerWithIdentifier identifier: String?
)
```

## Parameters 

`group`  

The group to add.

`identifier`  

The identifier of the container to add the new group. To add the new group to the default container, set `identifier` to `nil`.

## Discussion

This method overrides any previously made delete request for the group.

## See Also

### Saving group changes

func update(CNMutableGroup)

Updates an existing group in the contact store.

func delete(CNMutableGroup)

Deletes a group from the contact store.

func addMember(CNContact, to: CNGroup)

Adds a contact as a member of a group.

func removeMember(CNContact, from: CNGroup)

Removes a contact as a member of a group.

