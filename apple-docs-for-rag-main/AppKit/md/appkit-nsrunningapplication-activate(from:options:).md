

- AppKit
- NSRunningApplication
-  activate(from:options:) 

Instance Method

# activate(from:options:)

Attempts to activate the application using the specified options.

macOS 14.0+

``` source
func activate(
    from application: NSRunningApplication,
    options: NSApplication.ActivationOptions = []
) -> Bool
```

## Parameters 

`application`  

The application to activate.

`options`  

The options to use during activation.

## Return Value

Returns true if the request is allowed by the system, otherwise false.

## Discussion

Use this method to request app activation. Calling this method doesn’t guarantee app activation. For cooperative activation, the other application should call yieldActivation(to:) or equivalent prior to the target application invoking activate().

## See Also

### Activating applications

func activate(options: NSApplication.ActivationOptions) -> Bool

Attempts to activate the application using the specified options.

var isActive: Bool

Indicates whether the application is currently frontmost.

struct ActivationOptions

The following flags are for activate(options:).

var activationPolicy: NSApplication.ActivationPolicy

Indicates the activation policy of the application.

enum ActivationPolicy

Activation policies (used by activationPolicy) that control whether and how an app may be activated.

