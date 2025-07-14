

- AppKit
- NSApplication
-  NSApplication.ActivationPolicy 

Enumeration

# NSApplication.ActivationPolicy

Activation policies (used by activationPolicy) that control whether and how an app may be activated.

macOS

``` source
enum ActivationPolicy
```

## Topics

### Activation Policies

case regular

The application is an ordinary app that appears in the Dock and may have a user interface.

case accessory

The application doesn’t appear in the Dock and doesn’t have a menu bar, but it may be activated programmatically or by clicking on one of its windows.

case prohibited

The application doesn’t appear in the Dock and may not create windows or be activated.

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

### Configuring the Activation Policy

func activationPolicy() -> NSApplication.ActivationPolicy

Returns the app’s activation policy.

func setActivationPolicy(NSApplication.ActivationPolicy) -> Bool

Attempts to modify the app’s activation policy.

