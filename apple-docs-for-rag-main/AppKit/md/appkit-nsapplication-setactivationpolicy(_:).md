

- AppKit
- NSApplication
-  setActivationPolicy(\_:) 

Instance Method

# setActivationPolicy(\_:)

Attempts to modify the app’s activation policy.

macOS 10.6+

``` source
@MainActor
func setActivationPolicy(_ activationPolicy: NSApplication.ActivationPolicy) -> Bool
```

## Parameters 

`activationPolicy`  

The desired activation policy.

## Return Value

true if the policy switch succeded; otherwise, false.

## Discussion

You can set any activation policy in macOS 10.9 and later; in macOS 10.8 and earlier, you can only set the activation policy to `NSApplicationActivationPolicyProhibited` or `NSApplicationActivationPolicyRegular`.

## See Also

### Configuring the Activation Policy

func activationPolicy() -> NSApplication.ActivationPolicy

Returns the app’s activation policy.

enum ActivationPolicy

Activation policies (used by activationPolicy) that control whether and how an app may be activated.

