

- AppKit
- NSApplication
-  activationPolicy() 

Instance Method

# activationPolicy()

Returns the app’s activation policy.

macOS 10.6+

``` source
@MainActor
func activationPolicy() -> NSApplication.ActivationPolicy
```

## Return Value

The app’s current activation policy.

## See Also

### Configuring the Activation Policy

func setActivationPolicy(NSApplication.ActivationPolicy) -> Bool

Attempts to modify the app’s activation policy.

enum ActivationPolicy

Activation policies (used by activationPolicy) that control whether and how an app may be activated.

