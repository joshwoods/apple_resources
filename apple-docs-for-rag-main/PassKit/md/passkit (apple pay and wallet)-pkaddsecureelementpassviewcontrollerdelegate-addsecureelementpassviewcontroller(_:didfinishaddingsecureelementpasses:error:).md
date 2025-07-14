

- PassKit (Apple Pay and Wallet)
- PKAddSecureElementPassViewControllerDelegate
-  addSecureElementPassViewController(\_:didFinishAddingSecureElementPasses:error:) 

Instance Method

# addSecureElementPassViewController(\_:didFinishAddingSecureElementPasses:error:)

Tells the delegate when PassKit finishes adding one or more Secure Element passes.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
func addSecureElementPassViewController(
    _ controller: PKAddSecureElementPassViewController,
    didFinishAddingSecureElementPasses passes: [PKSecureElementPass]?,
    error: (any Error)?
)
```

**Required**

## Parameters 

`controller`  

The view controller that requests PassKit to add passes.

`passes`  

If addition succeeds, the array of Secure Element passes that PassKit adds; otherwise, `nil`.

`error`  

If addition fails, an error that describes the failure; otherwise, `nil`. See PKAddSecureElementPassError for more information.

## See Also

### Responding to pass addition

func addSecureElementPassViewController(PKAddSecureElementPassViewController, didFinishAdding: PKSecureElementPass?, error: (any Error)?)

Tells the delegate when PassKit finishes adding a Secure Element pass.

Deprecated

