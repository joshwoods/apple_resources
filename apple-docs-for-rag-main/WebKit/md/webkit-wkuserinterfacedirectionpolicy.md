

- WebKit
-  WKUserInterfaceDirectionPolicy 

Enumeration

# WKUserInterfaceDirectionPolicy

The policy that determines the directionality of user interface elements in a web view.

macOS 10.12+

``` source
enum WKUserInterfaceDirectionPolicy
```

## Overview

When `WKUserInterfaceDirectionPolicyContent` is specified, the directionality of user interface elements is affected by the `dir` attribute or the `direction` CSS property. When `WKUserInterfaceDirectionPolicySystem` is specified, the directionality of user interface elements is affected by the direction of the view.

## Topics

### Direction Policies

case content

The directionality follows the CSS/HTML/XHTML specifications.

case system

The directionality follows the view’s user interface layout direction.

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

### Selecting user interface directionality

var userInterfaceDirectionPolicy: WKUserInterfaceDirectionPolicy

The directionality of user interface elements.

