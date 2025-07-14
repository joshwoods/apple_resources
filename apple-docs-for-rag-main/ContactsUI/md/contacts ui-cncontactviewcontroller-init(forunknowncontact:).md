

- Contacts UI
- CNContactViewController
-  init(forUnknownContact:) 

Initializer

# init(forUnknownContact:)

Initializes a view controller for an unknown contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
convenience init(forUnknownContact contact: CNContact)
```

## Parameters 

`contact`  

The contact to be displayed.

## Return Value

A newly initialized CNContactViewController object.

## Discussion

This view controller initializes the customized behavior and appearance of CNContactViewController for an unknown contact.

## See Also

### Creating the Contact Viewer

convenience init(for: CNContact)

Initializes a view controller for an existing contact.

convenience init(forContact: CNContact)

Initializes a view controller for an existing contact.

convenience init(forNewContact: CNContact?)

Initializes a view controller for a new contact.

