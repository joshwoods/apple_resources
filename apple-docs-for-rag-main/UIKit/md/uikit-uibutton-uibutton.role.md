

- UIKit
- UIButton
-  UIButton.Role 

Enumeration

# UIButton.Role

Constants that describe the role of the button.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
enum Role
```

## Topics

### Button Roles

case normal

A button role for a default button style.

case primary

A button role that responds to a primary key press.

case cancel

A button role that responds to a cancel action.

case destructive

A button role with a red background color.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying the role

var role: UIButton.Role

The role of the button.

