

- PassKit (Apple Pay and Wallet)
- PKAddCarKeyPassConfiguration
-  password 

Instance Property

# password

A one-time password that the vehicle manufacturer provides.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOSvisionOS 1.0+

``` source
var password: String { get set }
```

## Discussion

When creating a digital car key, the vehicle manufacturer emails the user a one-time password to verify their identity. Set this property’s value to that password before you use the configuration to initialize PKAddSecureElementPassViewController, and PassKit verifies that the passwords match as it creates the pass.

