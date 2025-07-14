

- UIKit
- UIApplication
- UIApplication.ExtensionPointIdentifier
-  keyboard 

Type Property

# keyboard

The identifier for custom keyboards.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
static let keyboard: UIApplication.ExtensionPointIdentifier
```

## Discussion

To reject the use of custom keyboards in your app, specify this constant in your implementation of the application(_:shouldAllowExtensionPointIdentifier:) delegate method.

## See Also

### Disallowing specified app extension types

func application(UIApplication, shouldAllowExtensionPointIdentifier: UIApplication.ExtensionPointIdentifier) -> Bool

Asks the delegate to grant permission to use app extensions that are based on a specified extension point identifier.

struct ExtensionPointIdentifier

A structure that identifies types of extensions.

