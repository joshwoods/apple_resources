

- UIKit
- UIApplicationDelegate
-  application(\_:shouldAllowExtensionPointIdentifier:) 

Instance Method

# application(\_:shouldAllowExtensionPointIdentifier:)

Asks the delegate to grant permission to use app extensions that are based on a specified extension point identifier.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    shouldAllowExtensionPointIdentifier extensionPointIdentifier: UIApplication.ExtensionPointIdentifier
) -> Bool
```

## Parameters 

`application`  

Your shared app object.

`extensionPointIdentifier`  

A constant identifying an extension point.

## Return Value

false to disallow use of a specified app extension type, or true to allow use of the type.

## Mentioned in 

Configuring a custom keyboard interface

## Discussion

You can implement this method to reject a specified type of app extension, based on its extension point identifier, from use in your app. See Extension Point Identifier Constants in UIApplication.

If you do not implement this method, all app extension types are available for use in your app.

In iOS 8.0, the only type of app extension you can reject is the custom keyboard. For information on app extensions, see App Extension Programming Guide.

## See Also

### Disallowing specified app extension types

struct ExtensionPointIdentifier

A structure that identifies types of extensions.

static let keyboard: UIApplication.ExtensionPointIdentifier

The identifier for custom keyboards.

