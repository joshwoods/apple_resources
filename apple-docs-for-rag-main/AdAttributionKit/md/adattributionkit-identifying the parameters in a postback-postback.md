

- AdAttributionKit
-  Identifying the parameters in a postback 

Article

# Identifying the parameters in a postback

Interpret postback properties to understand the attribution report.

## Overview

The following list describes all the possible parameters you can get in a postback. To verify that Apple signed the postback, see Verifying a postback.

## Understand the JSON stanza the framework sends

The JSON stanza your servers receive resembles the following:

```
{
  "ad-interaction-type": "click",
  "jws-string": "eyJraWQiOiJhcHBsZS1jYXMtaWRlbnRpZmllci8wIiwiYWxnIjoiRVMyNTYifQ.eyJhZHZlcnRpc2VkLWl0ZW0taWRlbnRpZmllciI6Njg0OTM5LCJjb252ZXJzaW9uLXR5cGUiOiJyZS1lbmdhZ2VtZW50IiwibWFya2V0cGxhY2UtaWRlbnRpZmllciI6ImNvbS5hcHBsZS5BcHBTdG9yZSIsImFkLW5ldHdvcmstaWRlbnRpZmllciI6InRlc3QuYWRhdHRyaWJ1dGlvbmtpdCIsImltcHJlc3Npb24tdHlwZSI6ImFwcC1pbXByZXNzaW9uIiwicG9zdGJhY2stc2VxdWVuY2UtaW5kZXgiOjAsInNvdXJjZS1pZGVudGlmaWVyIjoiODM0NCIsImRpZC13aW4iOnRydWUsInBvc3RiYWNrLWlkZW50aWZpZXIiOiIzZjUwZmU1Ny0yOWFlLTQ4NjEtOGMwYi1hYzZhZGRkZmY3MmMiLCJwdWJsaXNoZXItaXRlbS1pZGVudGlmaWVyIjo1ODM4NDkyfQ.AemK1x2ahIPKOnFEEscG4wvipRtR1G6DzpNF4M4joPb8POIH4FJjm4VvcNgLXc9rWBrEDQPvDblduoc7MFcK5w",
  "coarse-conversion-value": "medium"
}
```

The keys in this stanza may include:

- conversion-value (optional) — An unsigned 6-bit value that the advertised app sets by calling a method to update the conversion value, such as updateConversionValue(_:lockPostback:).

- coarse-conversion-value (optional) — Possible values are the strings `low`, `medium`, and `high`. The advertised app sets this value by calling a method to update conversion values, such as updateConversionValue(_:coarseConversionValue:lockPostback:).

- ad-interaction-type - The string *view*, indicating that the postback is the result of a view-through impression, or the string *click*, indicating that it’s the result of a click-through impression.

- jws-string — A compact JSON web signature (JWS) of the Apple-signed postback contents.

## Examine the JWS header for the encryption algorithm and key identifier

The JWS header of the postback consists of two parameters and resembles the following structure:

```
{
  "kid": "apple-cas-identifier/0",
  "alg": "ES256"
}
```

The keys for this structure are:

- alg — The encryption algorithm Apple used to sign the postback.

- kid — The identifier of the key Apple used to sign the postback.

## Examine the JWS payload of the postback

The JWS decoded payload of the postback resembles the following structure:

```
{
  "advertised-item-identifier": 684939,
  "conversion-type": "re-engagement",
  "marketplace-identifier": "com.apple.AppStore",
  "ad-network-identifier": "test.adattributionkit",
  "impression-type": "app-impression",
  "postback-sequence-index": 0,
  "source-identifier": "8344",
  "did-win": true,
  "postback-identifier": "3f50fe57-29ae-4861-8c0b-ac6adddff72c",
  "publisher-item-identifier": 5838492
}
```

The keys the framework delivers in this structure may include the following:

- advertised-item-identifier — The app item ID of the advertised app.

- conversion-type — The string `download` that the system returns to indicate someone purchased and downloaded the app for the first time, or the string `redownload` to indicate someone downloaded an already-purchased app. The string `re-engagement` to indicate someone reengaged with an app that they previously installed.

- marketplace-identifier (optional) — The bundle ID of the alternative marketplace the advertised app was installed from.

- ad-network-identifier — The string that identifies the ad network.

- impression-type — The string `app-impression`.

- postback-sequence-index - The possible integer values of `0`, `1`, and `2` signify the order of postbacks that result from the three conversion windows. For more information, see Receiving postbacks in multiple conversion windows.

- source-identifier — The hierarchical source identifier with two, three, or four digits.

- did-win — A Boolean value that’s `true` if the ad network wins the attribution, or `false` if the postback represents a qualifying ad impression that doesn’t win the attribution.

- postback-identifier — The postback’s unique identifier.

- publisher-item-identifier (optional) — The app ID of the app that displays the ad.

## Examine the postback’s JWS signature

The signature is a combination of the JSON Web Signature (JWS) header and payload components that Apple signs using its private key.

For more information about verifying the postback’s signature, see Verifying a postback. For more information about receiving postbacks, see Receiving postbacks in multiple conversion windows.

## Understand the crowd anonymity controlled properties

To help ensure crowd anonymity, Apple assigns a postback data tier to app downloads. The postback data tier determines whether certain parameters appear in the postback, as well as the number of digits in the hierarchical source identifier. The following postback parameters are subject to the postback data tier:

- `coarse-conversion-value`

- `conversion-value`

- `source-identifier` (affects the number of digits the postback returns)

- `publisher-item-identifier`

- `marketplace-identifier`

## See Also

### Postback verification and parameter identification

Verifying a postback

Ensure the validity of a postback you receive after an ad conversion by verifying its cryptographic signature.

