

- SKAdNetwork for Web Ads
-  Generating a signature for attributable web ads 

Article

# Generating a signature for attributable web ads

Initiate install-validation by providing the signed parameters for an attributable web ad.

## Overview

A user’s device calls the Get a Signed Web Ad Impression Payload endpoint on your server when a user taps the web ad that you create using the instructions in Creating an attributable ad link. To respond to the request, you need to provide the values in the AdImpressionResponse, which includes a cryptographic signature.

To generate the signature, combine the required values from the signature object and cryptographically sign the resulting string. Use the ad network ID and PKCS#8 private key that you establish when registering to use the API. For more information, see Registering an ad network.

### Combine the parameters

Create the UTF-8 string using the required signature object parameters.

Important

Lowercase the string representation of the nonce from the signature object. Failing to do so results in an invalid signature. Only ads with valid signatures can get ad attributions.

Combine the values into a UTF-8 string with an invisible separator (`‘\u2063’`) between them, in the exact order the code below shows:

```
```

### Sign the combined string

Sign the combined UTF-8 string with the following key and algorithm:

- Your PKCS#8 private key.

- The Elliptic Curve Digital Signature Algorithm (ECDSA) with a SHA-256 hash.

The resulting Digital Encoding Rules (DER)-formatted binary value is the signature.

### Encode the signature

Encode the binary signature you generate into a Base64 string. The result is your ad network attribution signature. The signature string should look similar to the following:

```
```

For more information about Base64 encoding, see base64EncodedString(options:).

### Use the generated signature string

After you generate the signature, use this value in the `signature` parameter of the AdImpressionResponse. If the user installs and launches the advertised app, the attribution-winning ad network receives an install-validation postback. For more information about postbacks, see Verifying an install-validation postback.

## See Also

### Providing the web ad signature and response

object AdImpressionResponse

The response you provide that contains a signed payload for a clicked web ad.

object signature

The key-value pairs that ad networks use to cryptographically sign a web ad.

