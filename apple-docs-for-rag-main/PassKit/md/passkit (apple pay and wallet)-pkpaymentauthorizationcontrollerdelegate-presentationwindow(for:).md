

- PassKit (Apple Pay and Wallet)
- PKPaymentAuthorizationControllerDelegate
-  presentationWindow(for:) 

Instance Method

# presentationWindow(for:)

Returns the window in which to present a payment authorization sheet.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+watchOS 7.0+

**Mac Catalyst, visionOS**

``` source
func presentationWindow(for controller: PKPaymentAuthorizationController) -> UIWindow?
```

**macOS**

``` source
func presentationWindow(for controller: PKPaymentAuthorizationController) -> NSWindow?
```

**iOS, iPadOS, watchOS**

``` source
optional func presentationWindow(for controller: PKPaymentAuthorizationController) -> UIWindow?
```

## Parameters 

`controller`  

The controller for the payment authorization sheet.

## Return Value

The window in which to present the payment authorization sheet.

