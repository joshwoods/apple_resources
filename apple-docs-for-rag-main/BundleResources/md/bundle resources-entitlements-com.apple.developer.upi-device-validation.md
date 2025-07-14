

- Bundle Resources
- Entitlements
-  com.apple.developer.upi-device-validation 

Property List Key

# com.apple.developer.upi-device-validation

A Boolean value that indicates whether the app can use Unified Payments Interface (UPI) device enrollment.

iOS 17.0+iPadOS 17.0+

## Details 

Type  

boolean

## Attributes 

Default: `NO`

## Discussion

With this entitlement, you can use setUPIVerificationCodeSendCompletion:, which configures the instance of MFMessageComposeViewController with non-editable recipients and body fields.

You must be an account holder of a development team to get permission to use this entitlement. To request access, see UPI device validation Entitlement Request. Add the entitlement to your app in the Xcode property list editor. Set the entitlement’s type to Boolean, and the corresponding value to YES.

