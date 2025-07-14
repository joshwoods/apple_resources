

- Foundation
- NSError
-  helpAnchor 

Instance Property

# helpAnchor

A string to display in response to an alert panel help anchor button being pressed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var helpAnchor: String? { get }
```

## Discussion

The object in the user info dictionary for the key NSHelpAnchorErrorKey. If the user info dictionary doesn’t contain a value for NSHelpAnchorErrorKey, this property is `nil`.

If this property is non-`nil` for an error being presented by init(error:), the alert panel will include a help anchor button that can display this string.

