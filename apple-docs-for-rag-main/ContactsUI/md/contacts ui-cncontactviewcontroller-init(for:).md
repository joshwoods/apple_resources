

- Contacts UI
- CNContactViewController
-  init(for:) 

Initializer

# init(for:)

Initializes a view controller for an existing contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
convenience init(for contact: CNContact)
```

## Parameters 

`contact`  

The existing contact.

## Return Value

A newly initialized CNContactViewController object.

## Discussion

This view controller initializes the customized behavior and appearance of CNContactViewController for a contact.

## See Also

### Creating the Contact Viewer

convenience init(forContact: CNContact)

Initializes a view controller for an existing contact.

convenience init(forUnknownContact: CNContact)

Initializes a view controller for an unknown contact.

convenience init(forNewContact: CNContact?)

Initializes a view controller for a new contact.

