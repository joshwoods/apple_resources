

- UIKit
- UIApplicationShortcutIcon
-  init(type:) 

Initializer

# init(type:)

Creates a Home Screen quick action icon using a system-defined image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
convenience init(type: UIApplicationShortcutIcon.IconType)
```

## Parameters 

`type`  

The system-defined image to use for the icon. For a list of possible images, see the UIApplicationShortcutIcon.IconType enumeration.

## Return Value

A Home Screen quick action icon initialized with the specified system image.

## Discussion

Use this method to create icons for actions supported by the system. Users expect system-defined action images to be used only for the intended action.

## See Also

### Creating a quick action icon

convenience init(templateImageName: String)

Creates a Home Screen quick action icon based on an image in your app’s bundle, preferably in an asset catalog.

convenience init(systemImageName: String)

Creates a Home Screen quick action icon using a system symbol image.

convenience init(contact: CNContact)

Creates a Home Screen quick action icon from the picture for a contact or a monogram of the contact name if the picture is unavailable.

