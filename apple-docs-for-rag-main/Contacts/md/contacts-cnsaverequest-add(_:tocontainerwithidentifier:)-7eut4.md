

- Contacts
- CNSaveRequest
-  add(\_:toContainerWithIdentifier:) 

Instance Method

# add(\_:toContainerWithIdentifier:)

Adds the specified contact to the contact store.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func add(
    _ contact: CNMutableContact,
    toContainerWithIdentifier identifier: String?
)
```

## Parameters 

`contact`  

The new contact to add.

`identifier`  

The identifier of the container to add the new contact. To add the new contact to the default container set `identifier` to `nil`.

## Discussion

This method overrides any previously made deletion requests for the contact. The new contact may be modified by executing the save request.

## See Also

### Saving contact changes

func update(CNMutableContact)

Updates an existing contact in the contact store.

func delete(CNMutableContact)

Deletes a contact from the contact store.

