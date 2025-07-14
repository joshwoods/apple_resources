

- App Store Server API
-  storefrontCountryCodes 

Type

# storefrontCountryCodes

A list of storefront country codes you provide to limit the storefronts for a subscription-renewal-date extension.

App Store Server API 1.7+

``` source
[storefrontCountryCode] storefrontCountryCodes
```

## Attributes 

Maximum length: `3`

## Discussion

You provide the list of storefront country codes in the MassExtendRenewalDateRequest to limit the storefronts in which the App Store extends the subscription renewal date. To indicate that the extension applies in all storefronts, omit the storefrontCountryCodes object from the MassExtendRenewalDateRequest object.

## See Also

### Data types

type extendByDays

The number of days to extend the subscription renewal date.

type extendReasonCode

The code that represents the reason for the subscription-renewal-date extension.

string productId

The product identifier of the In-App Purchase.

type requestIdentifier

A string that contains a unique identifier you provide to track each subscription-renewal-date extension request.

type storefrontCountryCode

The three-letter code that represents the country or region associated with the App Store storefront.

