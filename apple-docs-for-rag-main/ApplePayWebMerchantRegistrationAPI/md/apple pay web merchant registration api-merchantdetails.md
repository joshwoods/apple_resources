

- Apple Pay Web Merchant Registration API
-  MerchantDetails 

Object

# MerchantDetails

Detailed information for a single registered merchant.

Apple Pay Web Merchant Registration API 1.0+

``` source
object MerchantDetails
```

## Properties

`domainNames`

`[string]`

A list of fully qualified domain names for which Apple Pay processes payments for this merchant.

`encryptTo`

`string`

A SHA-256 hash of the merchant ID that you provided for the `encrypTo` value when calling Register Merchant.

`partnerMerchantName`

`string`

A human-readable name for the merchant.

Maximum length: `1024`

`partnerMerchantValidationURI`

`string`

The URI used by Apple to locate the domain verification file during merchant registration. It is used for tracking and debugging.

`partnerInternalMerchantIdentifier`

`string`

The identifier that uniquely identifies the merchant.

Maximum length: `1024`

Value: `/ a-zA-Z0-9~-_+&@$!|,.;/`

## Discussion

To compare your merchant ID with the value that this request returns in the `encryptTo` string, create a SHA-256 hash of your merchant ID first. In the Terminal app, enter the following command, replacing `com.your.merchant.id` with your merchant ID:

```
echo -n com.your.merchant.id | openssl dgst -sha256
```

The result is a hexidecimal value that you can compare with the value that this request returns in the `encryptTo` string.

## See Also

### Web Merchant Details

Get Merchant Details

Retrieve information about a registered merchant’s current state by using the merchant’s internal merchant identifier.

