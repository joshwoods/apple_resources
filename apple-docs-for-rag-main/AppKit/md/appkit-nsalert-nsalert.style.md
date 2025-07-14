

- AppKit
- NSAlert
-  NSAlert.Style 

Enumeration

# NSAlert.Style

The set of alert styles to style alerts in your app.

macOS

``` source
enum Style
```

## Overview

Currently, there’s no visual difference between informational and warning alerts. You should only use the critical (or “caution”) alert style if warranted. For design guidance on alert styles, see Human Interface Guidelines > Alerts. The default alert style is NSAlert.Style.warning.

## Topics

### Enumeration Cases

case critical

An alert style to inform someone about a critical event.

case warning

An alert style to warn someone about a current or impending event.

case informational

An alert style to inform someone about a current or impending event.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct ModalResponse

A set of button return values for modal dialogs.

