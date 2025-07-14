

- Contacts UI
- CNContactViewController
-  contactStore 

Instance Property

# contactStore

The contact store from which the contact was fetched or to which it will be saved.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var contactStore: CNContactStore? { get set }
```

## Discussion

If not this property is not set, than adding the contact to the user’s contacts is disabled.

