

- AppKit
- NSRunningApplication
-  isActive 

Instance Property

# isActive

Indicates whether the application is currently frontmost.

macOS 10.6+

``` source
var isActive: Bool { get }
```

## Discussion

This property is observable using key-value observing.

## See Also

### Activating applications

func activate(options: NSApplication.ActivationOptions) -> Bool

Attempts to activate the application using the specified options.

func activate(from: NSRunningApplication, options: NSApplication.ActivationOptions) -> Bool

Attempts to activate the application using the specified options.

struct ActivationOptions

The following flags are for activate(options:).

var activationPolicy: NSApplication.ActivationPolicy

Indicates the activation policy of the application.

enum ActivationPolicy

Activation policies (used by activationPolicy) that control whether and how an app may be activated.

