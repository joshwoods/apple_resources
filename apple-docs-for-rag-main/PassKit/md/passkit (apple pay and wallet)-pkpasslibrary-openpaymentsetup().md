

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  openPaymentSetup() 

Instance Method

# openPaymentSetup()

Opens the user interface to set up credit cards for Apple Pay.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+

``` source
func openPaymentSetup()
```

## Discussion

Use this method to move users to the interface for adding credit cards. This method transfers control to the Wallet app on iPhone or to the Settings app on iPad. For devices that don’t support Apple Pay, this method does nothing.

