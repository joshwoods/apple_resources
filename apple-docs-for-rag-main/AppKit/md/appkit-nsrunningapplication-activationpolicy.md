

- AppKit
- NSRunningApplication
-  activationPolicy 

Instance Property

# activationPolicy

Indicates the activation policy of the application.

macOS 10.6+

``` source
var activationPolicy: NSApplication.ActivationPolicy { get }
```

## Discussion

The value returned by this property is usually fixed, but it may change through a call to activate(options:).

This property is observable using key-value observing.

## See Also

### Activating applications

func activate(options: NSApplication.ActivationOptions) -> Bool

Attempts to activate the application using the specified options.

func activate(from: NSRunningApplication, options: NSApplication.ActivationOptions) -> Bool

Attempts to activate the application using the specified options.

var isActive: Bool

Indicates whether the application is currently frontmost.

struct ActivationOptions

The following flags are for activate(options:).

enum ActivationPolicy

Activation policies (used by activationPolicy) that control whether and how an app may be activated.

