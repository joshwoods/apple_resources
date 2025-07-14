

- PassKit (Apple Pay and Wallet)
- PKAddSecureElementPassViewControllerDelegate
-  addSecureElementPassViewController(\_:didFinishAdding:error:) Deprecated

Instance Method

# addSecureElementPassViewController(\_:didFinishAdding:error:)

Tells the delegate when PassKit finishes adding a Secure Element pass.

iOS 13.4–14.0DeprecatediPadOS 13.4–14.0DeprecatedMac Catalyst 13.4–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func addSecureElementPassViewController(
    _ controller: PKAddSecureElementPassViewController,
    didFinishAdding pass: PKSecureElementPass?,
    error: (any Error)?
)
```

Deprecated

Use addSecureElementPassViewController(_:didFinishAddingSecureElementPasses:error:) instead.

## Parameters 

`controller`  

The view controller that requests PassKit to add a pass.

`pass`  

If addition succeeds, the Secure Element pass that PassKit adds; otherwise, `nil`.

`error`  

If addition fails, an error that describes the failure; otherwise, `nil`. See PKAddSecureElementPassError for more information.

## See Also

### Responding to pass addition

func addSecureElementPassViewController(PKAddSecureElementPassViewController, didFinishAddingSecureElementPasses: [PKSecureElementPass]?, error: (any Error)?)

Tells the delegate when PassKit finishes adding one or more Secure Element passes.

**Required**

