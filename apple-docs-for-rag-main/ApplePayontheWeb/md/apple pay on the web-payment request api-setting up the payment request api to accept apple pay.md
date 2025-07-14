

- Apple Pay on the Web
- Payment Request API
-  Setting up the payment request API to accept Apple Pay 

Article

# Setting up the payment request API to accept Apple Pay

Support payments using Apple Pay on your website.

## Overview

Throughout the W3C Payment Request API specification, properties and attributes with the type `object` contain specific data related to payment methods. When using Apple Pay, keep in mind that these properties and attributes with the type `object` have a concrete type.

To indicate that data is specific to Apple Pay, set the supportedMethods property of the W3C PaymentMethodData dictionary and W3C PaymentDetailsModifier dictionary to the Apple Pay URL `https://apple.com/apple-pay`.

Set up the payment request by setting the data property of the W3C PaymentMethodData dictionary to an ApplePayRequest dictionary. The following is an example of an ApplePayRequest dictionary that requires Apple Pay Version 12:

```
let applePayPaymentMethodData = {
    supportedMethods: "https://apple.com/apple-pay",
    data: {
        version: 12,
        // Add additional ApplePayRequest attributes here.
    },
};
```

Customize the payment request by setting the data property of the W3C PaymentDetailsModifier dictionary to an ApplePayModifier dictionary. The following is an example of an ApplePayModifier dictionary that only applies to credit cards:

```
let applePayPaymentDetailsModifier = {
    supportedMethods: "https://apple.com/apple-pay",
    data: {
        paymentMethodType: "credit",
        // Add additional ApplePayModifier attributes here.
    },
};
```

Handle changes made by the user to features specific to Apple Pay by looking at the methodDetails attribute of the W3C PaymentMethodChangeEvent:

- If the user changes the payment method type, the methodDetails attribute is an ApplePayPaymentMethod dictionary.

- If the user changes the coupon code, the methodDetails attribute is an ApplePayCouponCodeDetails dictionary.

The following is an example of how to differentiate these different scenarios when handling a W3C PaymentMethodChangeEvent:

```
paymentRequest.addEventListener("paymentmethodchange", function(event) {
    if (event.methodName === "https://apple.com/apple-pay") {
        if (event.methodDetails.couponCode) {
            let applePayCouponCodeDetails = event.methodDetails;
            // Handle coupon code updates here.
            return;
        }

        let applePayPaymentMethodDetails = event.methodDetails;
        if (applePayPaymentMethodDetails.type === "credit") {
            // Handle credit payment method type changes here.
        } else {
            // Handle other payment method type changes here.
        }
    }
});
```

Explain issues by creating custom error messages using an array of ApplePayError objects:

- If the user makes any problematic changes, set the paymentMethodErrors property of the W3C PaymentDetailsUpdate dictionary.

- If a problem occurs during authorization, set the paymentMethod property of the W3C PaymentValidationErrors dictionary.

The following is an example of how to show custom error messages if the user inputs an invalid coupon code or shipping postal code:

```
paymentRequest.addEventListener("shippingaddresschange", function(event) {
    if (event.methodName === "https://apple.com/apple-pay") {
        if (event.methodDetails.couponCode) {
            let applePayCouponCodeDetails = event.methodDetails;
            if (!isValidCouponCode(applePayCouponCodeDetails.couponCode) {
                event.updateWith({
                    paymentMethodErrors: [
                        new ApplePayError("couponCodeInvalid", undefined, "Coupon code is invalid"),
                    ],
                });
                return;
            }

            // Handle valid coupon code updates here.
            return;
        }

        let applePayPaymentMethodDetails = event.methodDetails;
        if (applePayPaymentMethodDetails.type === "credit") {
            // Handle credit payment method type changes here.
        } else {
            // Handle other payment method type changes here.
        }
    }
});

paymentRequest.show().then(function(paymentResponse) {
    if (paymentResponse.methodName === "https://apple.com/apple-pay") {
        if (!hasValidShippingZIPCode(paymentResponse)) {
            paymentResponse.retry({
                paymentMethod: [
                    new ApplePayError("shippingContactInvalid", "postalCode", "ZIP Code is invalid"),
                ],
            });
            return;
        }

        // Handle authorization with valid details here.
    }
});

```

Get the payment information after the user authorizes the payment request by looking at the details attribute of the W3C PaymentResponse, which is an ApplePayPayment dictionary. The following example accesses the postalCode after authorization:

```
function hasValidShippingZIPCode(paymentResponse) {
    if (paymentResponse.methodName === "https://apple.com/apple-pay") {
        let applePayPayment = paymentResponse.details;
        let shippingZIPCode = applePayPayment.shippingContact.postalCode;
        // Validate shipping ZIP code here.
    }
}
```

## See Also

### Payment request

ApplePayRequestBase

A dictionary that defines basic payment and contact information that the Apple Pay payment request object uses for the W3C Payment Request API.

ApplePayRequest

A dictionary that defines the Apple Pay payment request object to use for the W3C Payment Request API.

ApplePayModifier

A dictionary that defines the Apple Pay modifiers for a payment type in the W3C Payment Request API.

ApplePayPaymentCompleteDetails

