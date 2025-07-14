

- UIKit
- UIApplicationShortcutIcon
-  init(contact:) 

Initializer

# init(contact:)

Creates a Home Screen quick action icon from the picture for a contact or a monogram of the contact name if the picture is unavailable.

iOS 9.0+iPadOS 9.0+visionOS 1.0+

``` source
convenience init(contact: CNContact)
```

## Parameters 

`contact`  

The CNContact contact object to derive the icon from.

## Return Value

A Home Screen quick action icon initialized with the contact’s picture or monogram.

## Discussion

To use this method, pass in a contact from the user’s contacts database, available through the CNContactStore object. If the contact you specify has a picture, the system creates a full-color quick action icon from that picture. If the contact has no picture, the system employs the contact’s initials and displays instead a monogram.

Note

This method employs the Contacts framework.

You can, alternatively, pass in a CNContact object you create at runtime. Such a contact must have at least a first name or a last name. The quick action icon returned from this method is then a monogram built from the contact’s name. With this approach, it isn’t possible for you to provide an image for the quick action icon.

Finally, you can call this method with an empty contact that you create by using the CNContact class’s inherited alloc and `init` methods. With this approach, the resulting icon is a monochrome silhouette.

When providing a set of contact quick actions, ensure that every one of them has an icon. This ensures the best appearance for the set of quick actions.

## See Also

### Creating a quick action icon

convenience init(type: UIApplicationShortcutIcon.IconType)

Creates a Home Screen quick action icon using a system-defined image.

convenience init(templateImageName: String)

Creates a Home Screen quick action icon based on an image in your app’s bundle, preferably in an asset catalog.

convenience init(systemImageName: String)

Creates a Home Screen quick action icon using a system symbol image.

