

- Contacts UI
- CNContactViewController
-  descriptorForRequiredKeys() 

Type Method

# descriptorForRequiredKeys()

Returns the descriptor for all the keys that must be fetched on the contact before setting it on the view controller.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
@MainActor
class func descriptorForRequiredKeys() -> any CNKeyDescriptor
```

## Return Value

Descriptor for all the keys that must be fetched.

## Discussion

Pass this descriptor to the `keysToFetch` of the CNContactFetchRequest if you want to display the contact in a CNContactViewController.

