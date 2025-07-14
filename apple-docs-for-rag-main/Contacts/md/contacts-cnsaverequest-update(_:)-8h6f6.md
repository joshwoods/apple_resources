

- Contacts
- CNSaveRequest
-  update(\_:) 

Instance Method

# update(\_:)

Updates an existing group in the contact store.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func update(_ group: CNMutableGroup)
```

## Parameters 

`group`  

The group to update.

## Discussion

The group to be updated must already exist in the contact store. If it does not, the update request fails, the `CNErrorCodeRecordDoesNotExist` error is thrown, and the `CNErrorUserInfoAffectedRecordsKey` array is updated to contain that object.

## See Also

### Saving group changes

func add(CNMutableGroup, toContainerWithIdentifier: String?)

Adds a group to the contact store.

func delete(CNMutableGroup)

Deletes a group from the contact store.

func addMember(CNContact, to: CNGroup)

Adds a contact as a member of a group.

func removeMember(CNContact, from: CNGroup)

Removes a contact as a member of a group.

