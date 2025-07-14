

- PassKit (Apple Pay and Wallet)
- PKDisbursementRequest
-  init(merchantIdentifier:currency:region:supportedNetworks:merchantCapabilities:summaryItems:) 

Initializer

# init(merchantIdentifier:currency:region:supportedNetworks:merchantCapabilities:summaryItems:)

Creates a disbursement request with the parameters you specify.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS

``` source
convenience init(
    merchantIdentifier: String,
    currency: Locale.Currency,
    region: Locale.Region,
    supportedNetworks: [PKPaymentNetwork],
    merchantCapabilities: PKMerchantCapability,
    summaryItems: [PKPaymentSummaryItem]
)
```

## Parameters 

`merchantIdentifier`  

A string that identifies the merchant.

`currency`  

The Locale.Currency that represents the ISO 4127 currency code, which represents the value of this disbursement.

`region`  

The Locale.Region that represents the merchant’s ISO 3166 region code.

`supportedNetworks`  

An array of PKPaymentNetwork networks the merchant supports.

`merchantCapabilities`  

An array of PKMerchantCapability structures that describe the capabilities the merchant supports.

`summaryItems`  

An array of PKPaymentSummaryItem objects that describe the disbursement.

