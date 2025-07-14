

- StoreKit
- Ad network attribution
- SKAdNetwork
-  Generating the signature to validate StoreKit-rendered ads 

Article

# Generating the signature to validate StoreKit-rendered ads

Initiate install validation by displaying a StoreKit-rendered ad with signed parameters.

## Overview

Install validation informs an ad network when users install and launch an app they purchase after viewing an ad. Ad networks first provide an ad with cryptographically signed information that includes their ad network ID. Later, if the ad results in a conversion, the customer’s device sends install-validation postbacks. For information about attribution-winning and nonwinning postbacks, see Receiving ad attributions and postbacks.

Note

These instructions are for signing StoreKit-rendered ads. If you’re presenting a view-through ad, see Generating the signature to validate view-through ads.

To display a StoreKit-rendered ad and initiate a validation, an app needs to call loadProduct(withParameters:completionBlock:) with a signature key that the ad network generates, SKStoreProductParameterAdNetworkAttributionSignature. To generate the signature, combine the required values from Ad network install-validation keys and cryptographically sign the resulting string. Use the ad network ID and PKCS#8 private key that you establish when registering to use the API. For more information, see Registering an ad network.

### Choose parameters based on signature version

Select the required values of Ad network install-validation keys based on the version of the signature you’re generating. The API supports multiple versions of signed ads. Use the most recent version available in the SDK whenever possible. For information about availability, see SKAdNetwork release notes.

The following table lists the required signature parameters for version 4 and later. Combine them in a UTF-8 string as the example shows in the Combine the parameters section below.

| Signature parameter | Equivalent key |
|----|----|
| `version` | SKStoreProductParameterAdNetworkVersion |
| `ad-network-id` | SKStoreProductParameterAdNetworkIdentifier |
| `source-identifier` | SKStoreProductParameterAdNetworkSourceIdentifier This value replaces SKStoreProductParameterAdNetworkCampaignIdentifier from previous versions. |
| `itunes-item-id` | SKStoreProductParameterITunesItemIdentifier |
| `nonce` | SKStoreProductParameterAdNetworkNonce  Lowercase the string representation of the nonce value in the signature. |
| `source-app-id` | SKStoreProductParameterAdNetworkSourceAppStoreIdentifier  During testing, use an ID of `0` if you’re using a development-signed build and not an app from the App Store. |
| `fidelity-type` | Version 2.2 and later signatures require this parameter.  Set `fidelity-type` to `1` for StoreKit-rendered ads. |
| `timestamp` | SKStoreProductParameterAdNetworkTimestamp |

To create signatures for previous SKAdNetwork versions, see:

- Combining parameters to generate signatures for SKAdNetwork 2.2 and 3.

- Combining parameters to generate a signature for SKAdNetwork 2.

- If you build your app with iOS SDK 11.3 through 13.7, see Combining parameters to generate a signature for SKAdNetwork 1.

#### Combine the parameters

Create the UTF-8 string using the parameters in the example below.

Important

Lowercase the string representation of the nonce: SKStoreProductParameterAdNetworkNonce. Failing to do so results in an invalid signature. Only ads with valid signatures can get ad attributions.

For version 4 and later, combine the values into a UTF-8 string with an invisible separator (`‘\u2063’`) between them, in the exact order the code below shows:

```
// Parameter values combined, in order, for version 4 and later.
version + '\u2063' + ad-network-id + '\u2063' + source-identifier + '\u2063' + itunes-item-id + '\u2063' + nonce + '\u2063' + source-app-id + '\u2063' + fidelity-type + '\u2063' + timestamp

```

### Sign the combined string

Sign the combined UTF-8 string with the following key and algorithm:

- Your PKCS#8 private key.

- The Elliptic Curve Digital Signature Algorithm (ECDSA) with a SHA-256 hash.

The resulting Digital Encoding Rules (DER)-formatted binary value is the signature.

### Encode the signature

Encode the binary signature you generate into a Base64 string. The result is your ad network attribution signature, SKStoreProductParameterAdNetworkAttributionSignature. The signature string should look similar to the following:

```
MEQCIEQlmZRNfYzKBSE8QnhLTIHZZZWCFgZpRqRxHss65KoFAiAJgJKjdrWdkLUOCCjuEx2RmFS7daRzSVZRVZ8RyMyUXg==
```

For more information about Base64 encoding, see base64EncodedString(options:).

### Use the generated signature string

After you generate the signature, you have all the required Ad network install-validation keys an app needs to call loadProduct(withParameters:completionBlock:) to intiate a validation.

If the user installs and launches the advertised app, the attribution-winning ad network receives an install-validation postback. For more information about postbacks, see Verifying an install-validation postback.

## Topics

### Signatures for SKAdNetwork 1, 2, and 2.2–3

Combining parameters to generate signatures for SKAdNetwork 2.2 and 3

Generate signatures to sign your ad with versions 2.2 and 3.

Combining parameters to generate a signature for SKAdNetwork 2

Generate signatures to sign your ad with version 2.

Combining parameters to generate a signature for SKAdNetwork 1

Generate signatures for apps compiled with earlier SDKs.

## See Also

### Signing StoreKit-rendered ads

Ad network install-validation keys

Specify key values that validate and associate an app installation with an ad campaign.

