

- Contacts UI
- CNContactViewController
-  init(forNewContact:) 

Initializer

# init(forNewContact:)

Initializes a view controller for a new contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
convenience init(forNewContact contact: CNContact?)
```

## Parameters 

`contact`  

The contact to be displayed.

## Return Value

A newly initialized CNContactViewController object.

## Discussion

This view controller initializes the customized behavior and appearance of CNContactViewController for a new contact.

## See Also

### Creating the Contact Viewer

convenience init(for: CNContact)

Initializes a view controller for an existing contact.

convenience init(forContact: CNContact)

Initializes a view controller for an existing contact.

convenience init(forUnknownContact: CNContact)

Initializes a view controller for an unknown contact.

