

- UIKit
- UICommandAlternate
-  init(coder:) 

Initializer

# init(coder:)

Creates a command alternative from data in an unarchiver.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init?(coder: NSCoder)
```

## See Also

### Creating a command alternative

convenience init(title: String, action: Selector, modifierFlags: UIKeyModifierFlags)

Creates a command alternative with the specified title, action, and modifier flags.

