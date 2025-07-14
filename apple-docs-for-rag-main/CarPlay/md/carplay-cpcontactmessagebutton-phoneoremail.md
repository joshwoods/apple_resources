

- CarPlay
- CPContactMessageButton
-  phoneOrEmail 

Instance Property

# phoneOrEmail

The contact’s phone number or email address.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var phoneOrEmail: String { get }
```

## Discussion

When a user taps a contact message button, Siri launches the compose message flow and uses this property’s value as the recipient’s contact information.

