

- User Notifications
- UNNotificationActionIcon
-  init(systemImageName:) 

Initializer

# init(systemImageName:)

Creates an action icon by using a system symbol image.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
convenience init(systemImageName: String)
```

## Parameters 

`systemImageName`  

The name of the system symbol image. Use the SF Symbols app to look up the names of system symbol images. Download this app from the design resources page at developer.apple.com.

## Return Value

An action icon that the system initializes with the system symbol image that your app specifies.

## See Also

### Essentials

convenience init(templateImageName: String)

Creates an action icon based on an image in your app’s bundle, preferably in an asset catalog.

