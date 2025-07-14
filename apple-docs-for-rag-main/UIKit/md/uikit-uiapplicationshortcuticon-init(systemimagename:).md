

- UIKit
- UIApplicationShortcutIcon
-  init(systemImageName:) 

Initializer

# init(systemImageName:)

Creates a Home Screen quick action icon using a system symbol image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
convenience init(systemImageName: String)
```

## Parameters 

`systemImageName`  

The name of the system symbol image. Use the SF Symbols app to look up the names of system symbol images. You can download this app from the design resources page at developer.apple.com.

## Return Value

A Home Screen quick action icon initialized with the specified system symbol image.

## See Also

### Creating a quick action icon

convenience init(type: UIApplicationShortcutIcon.IconType)

Creates a Home Screen quick action icon using a system-defined image.

convenience init(templateImageName: String)

Creates a Home Screen quick action icon based on an image in your app’s bundle, preferably in an asset catalog.

convenience init(contact: CNContact)

Creates a Home Screen quick action icon from the picture for a contact or a monogram of the contact name if the picture is unavailable.

