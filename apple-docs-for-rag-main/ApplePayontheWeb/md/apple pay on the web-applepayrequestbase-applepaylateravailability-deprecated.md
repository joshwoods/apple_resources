

- Apple Pay on the Web
- ApplePayRequestBase
-  applePayLaterAvailability Deprecated

Instance Property

# applePayLaterAvailability

A value that indicates whether Apple Pay Later is available for a transaction.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayLaterAvailability applePayLaterAvailability;
```

Deprecated

Apple Pay Later is deprecated.

## Discussion

Use this property to suppress Apple Pay Later for a specific transaction. Only set this property if you have a specific requirement to disable Apple Pay Later.

Ensure you select the correct mode that matches your requirement, because the framework displays Apple Pay Later availability to the your customers.

Important

If you later decide to stop providing Apple Pay Later in your app, contact your acquirer or payment service provider (PSP) and notify them that you no longer wish to participate in the Mastercard Installments Program. You can always change this decision later.

## See Also

### Setting the Apple Pay Later mode

ApplePayLaterAvailability

Values you use to enable or disable Apple Pay Later for a specific transaction.

Deprecated

