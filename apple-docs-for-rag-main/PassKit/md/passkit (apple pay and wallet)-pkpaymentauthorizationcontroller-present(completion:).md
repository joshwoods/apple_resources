

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationController
-  present(completion:) 

Instance Method

# present(completion:)

Presents the payment sheet modally over your app.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
func present(completion: ((Bool) -> Void)? = nil)
```

``` source
func present() async -> Bool
```

## Parameters 

`completion`  

A block that is called after the sheet is presented. This block is passed the following parameters:

success  
A Boolean value that indicates whether the payment sheet was successfully presented. true if the payment sheet was presented successfully; otherwise, false.

## Discussion

You are responsible for dismissing the payment sheet.

## See Also

### Handling user interactions

var delegate: (any PKPaymentAuthorizationControllerDelegate)?

The controller’s delegate.

protocol PKPaymentAuthorizationControllerDelegate

Methods that let you respond to user interactions with your payment authorization controller.

func dismiss(completion: (() -> Void)?)

Dismisses the payment sheet.

