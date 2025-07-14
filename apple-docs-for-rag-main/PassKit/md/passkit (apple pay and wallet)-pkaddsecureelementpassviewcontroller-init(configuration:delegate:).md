

- PassKit (Apple Pay and Wallet)
- PKAddSecureElementPassViewController
-  init(configuration:delegate:) 

Initializer

# init(configuration:delegate:)

Creates a view controller using the specified pass configuration.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
init?(
    configuration: PKAddSecureElementPassConfiguration,
    delegate: (any PKAddSecureElementPassViewControllerDelegate)?
)
```

## Parameters 

`configuration`  

The configuration that the view controller uses to create a Secure Element pass.

`delegate`  

An object that acts as the view controller’s delegate.

## Discussion

The delegate must adopt the PKAddSecureElementPassViewControllerDelegate protocol. The view controller doesn’t retain the delegate.

