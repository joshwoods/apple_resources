

- Security
- SecAccessControlCreateFlags
-  userPresence 

Type Property

# userPresence

Constraint to access an item with either biometry or passcode.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var userPresence: SecAccessControlCreateFlags { get }
```

## Mentioned in 

Restricting keychain item accessibility

## Discussion

Biometry doesn’t have to be available or enrolled. The item is still accessible by Touch ID even if fingers are added or removed, or by Face ID if the user is re-enrolled.

This option is equivalent to specifying biometryAny, or, and devicePasscode.

