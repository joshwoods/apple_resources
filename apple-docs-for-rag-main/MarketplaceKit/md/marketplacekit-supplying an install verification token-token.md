

- MarketplaceKit
-  Supplying an install verification token 

Article

# Supplying an install verification token

Support the installation of alternative distribution apps by creating signed JSON web tokens.

## Overview

To enable app downloads from your website or alternative app marketplace using MarketplaceKit, your web server supplies a special secure element, or *install verification token*, to the device’s operating system through the app installation process.

An install verification token is a JSON web signature (JWS), or *signed* JSON web token (JWT). The token contains data that the system needs to verify the installation, such as the marketplace that installs it, if applicable, and the time the installation occurs. Create the token and sign it with your alternative distribution key set up with App Store Connect. For more information about JWTs, see RFC 7519.

The following app download situations require you to create an install verification token:

- MarketplaceKitURIScheme requests on webpages that distribute an app; see Installing your app from your website.

- AppLibrary methods that install apps from within a marketplace app, for example, requestAppInstallation(for:account:installVerificationToken:).

- ActionButton, through an LAContext; see Installing apps from an alternative marketplace.

## Create the JSON web token

To create the JWT, define a JWT header and provide key details in the payload.

Use the following table to complete the header details:

| Header key | Value |
|----|----|
| `alg` | The signing algorithm, `"ES256"`. |
| `kid` | *key ID*. A UUID for the alternative distribution public key associated to the app being downloaded. An alternative app marketplace has a single set of alternative distribution keys. Other apps that install over the web require a set of alternative distribution keys per app. If the app being downloaded installs from an alternative app marketplace, use the marketplace’s distribution keys. Set this value to the `data.id` property of the Read an app’s alternative distribution key endpoint response. For more information on alternative distribution keys, see Alternative Distribution Keys. |
| `typ` | The communication type, `"JWT"`. |

Next, define the JWT payload. Among the data to include are the issuer, bundle ID, expiration time, and nonce. Use the following table to fill in the payload:

| Payload key | Value |
|----|----|
| `iss` | *issuer*. A `String` representation of the AppleItemID for the installing alternative marketplace, or other app that installs from a website. |
| `iat` | *issued at*. The time at which you generate the token, as the `Int` number of seconds since January 1, 1970 00:00:00 UTC. |
| `exp` | *expiration*. The time after which the token expires, as the `Int` number of seconds since January 1, 1970 00:00:00 UTC. |
| `aud` | *audience*. The token recipient. Enter `AppleDownloadVerification-v1`. |
| `bid` | The bundle identifier of the app to install. |
| `dtype` | The record of previous downloads. Enter `download` the first time the app installs on a particular device and `redownload` for subsequent installs. Your web server needs to track the `dtype` of every install and set an accurate value. AdAttributionKit makes this information available to advertisers. |
| `nonce` | A randomly generated UUID as a `String` that acts as an anti-replay value. |
| `iid` | *item ID* (optional). The AppleItemID of the app the system is installing as a `String`. This value enhances app installation performance, when present. |
| `vid` | *version ID* (optional). The AppleVersionID of the app the system is installing as a `String`. This value enhances app installation performance, when present. |

An example JWT follows:

```
{
   "alg": "ES256",
   "kid": "52c5cb04-1163-4a30-ad4f-a3433cd6a4f6",
   "typ": "JWT"
}
{
   "iss": "1234123412",
   "iat": 1623085200,
   "exp": 1623086400,
   "aud": "AppleDownloadVerification-v1",
   "bid":  "com.example.mytestapp",
   "dtype" : "download",
   "nonce": "9BC2C5CC-A1F8-4F93-9D6A-4D524685B67E"
}
```

For sample code and open source tools that assist with JWT creation, see JWT.io.

## Sign the token and return it in response

To sign the token, use:

- Elliptic Curve Digital Signature Algorithm (ECDSA) with the P-256 curve and the SHA-256 hash algorithm.

- Your alternative distribution private key. For more information about the alternative distribution keys, see Creating keys and establishing alternative marketplace connections.

You can call an installation function either within an alternative app marketplace, or a webpage. Either way, your web server fields the JWT request by generating a token, signing it, and returning it to the call site.

## See Also

### Web services

Processing alternative app marketplace notifications

Manage the addition and removal of apps available on your alternative marketplace.

Ingesting an alternative distribution package

Process an available app version from App Store Connect and store it for download from your server.

Installing your app from your website

Manage the installation of an app that you develop and distribute through your website.

Installing apps from an alternative marketplace

Manage the installation of apps that developers distribute from your marketplace app.

