

- AppKit
- NSRunningApplication
-  activate(options:) 

Instance Method

# activate(options:)

Attempts to activate the application using the specified options.

macOS 10.6+

``` source
func activate(options: NSApplication.ActivationOptions = []) -> Bool
```

## Parameters 

`options`  

The options to use when activating the application. See NSApplication.ActivationOptions for the possible values.

## Return Value

true if the application was activated successfully, otherwise false.

## Discussion

This method will return false if the application has quit, or is not a type of application than can be activated.

## See Also

### Activating applications

func activate(from: NSRunningApplication, options: NSApplication.ActivationOptions) -> Bool

Attempts to activate the application using the specified options.

var isActive: Bool

Indicates whether the application is currently frontmost.

struct ActivationOptions

The following flags are for activate(options:).

var activationPolicy: NSApplication.ActivationPolicy

Indicates the activation policy of the application.

enum ActivationPolicy

Activation policies (used by activationPolicy) that control whether and how an app may be activated.

