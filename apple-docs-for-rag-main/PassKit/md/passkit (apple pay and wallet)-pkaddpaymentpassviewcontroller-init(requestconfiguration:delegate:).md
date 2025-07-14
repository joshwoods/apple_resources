

- PassKit (Apple Pay and Wallet)
- PKAddPaymentPassViewController
-  init(requestConfiguration:delegate:) 

Initializer

# init(requestConfiguration:delegate:)

Returns an initialized add payment view controller object, using the provided configuration and delegate.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init?(
    requestConfiguration configuration: PKAddPaymentPassRequestConfiguration,
    delegate: (any PKAddPaymentPassViewControllerDelegate)?
)
```

## Parameters 

`configuration`  

A configuration object that defines the view controller’s appearance.

`delegate`  

The add payment view controller’s delegate.

## Return Value

A newly initialized add payment view controller.

## Discussion

Adding payment passes requires a special entitlement issued by Apple. If your app does not include this entitlement, this method returns `nil`. For more information on requesting this entitlement, see the Card Issuers section on developer.apple.com/apple-pay/.

## See Also

### Creating an add-payment-pass view controller

class PKAddPaymentPassRequestConfiguration

Contains the configuration data for a view controller that lets the user add a payment pass.

