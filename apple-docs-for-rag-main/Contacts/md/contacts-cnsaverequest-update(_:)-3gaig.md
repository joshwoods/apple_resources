

- Contacts
- CNSaveRequest
-  update(\_:) 

Instance Method

# update(\_:)

Updates an existing contact in the contact store.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func update(_ contact: CNMutableContact)
```

## Parameters 

`contact`  

The contact to update.

## Discussion

The contact to be updated must already exist in the contact store. If it does not, the update request fails, the `CNErrorCodeRecordDoesNotExist` error occurs, and the `CNErrorUserInfoAffectedRecordsKey` array is updated to contain the object. Note that the contact may be modified when the save request is executing.

## See Also

### Saving contact changes

func add(CNMutableContact, toContainerWithIdentifier: String?)

Adds the specified contact to the contact store.

func delete(CNMutableContact)

Deletes a contact from the contact store.

