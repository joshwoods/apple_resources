

- UIKit
- UIPreviewAction
-  UIPreviewAction.Style Deprecated

Enumeration

# UIPreviewAction.Style

The style for a peek quick action.

iOS 9.0–17.1DeprecatediPadOS 9.0–17.1DeprecatedMac Catalyst 13.1–17.1DeprecatedtvOS 9.0–17.1Deprecated

``` source
enum Style
```

## Overview

Use these styles with instances of the UIPreviewAction and UIPreviewActionGroup classes.

## Topics

### Constants

case `default`

The default style.

case selected

The style for a selected peek quick action.

case destructive

The style for a peek quick action that changes or deletes data.

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

### Creating a peek quick action

convenience init(title: String, style: UIPreviewAction.Style, handler: (UIPreviewAction, UIViewController) -> Void)

Creates a peek quick action using a specified title, style, and handler.

Deprecated

var handler: (any UIPreviewActionItem, UIViewController) -> Void

The block called when the peek quick action is selected by the user.

Deprecated

