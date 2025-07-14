

- SKAdNetwork for Web Ads
-  Creating an attributable ad link 

Article

# Creating an attributable ad link

Create click-through web ads that attribute App Store app installations to your ad network.

## Overview

The web provides a broad platform for advertising apps to a wide audience. In iOS 16.1 and later, ad networks can use the SKAdNetwork for Web Ads API to get SKAdNetwork attributions for App Store app installations that originate from web ads in Safari.

### Register an ad network

Before creating an attributable ad link, you need to register your ad network with Apple. For information, see Registering an ad network.

### Create a link with the expected format

To receive app-installation attribution from a web ad, provide a specialized link that directs a person to download the advertised app from the App Store. The link needs to be in the following format:

```
```

Provide the following values to retrieve the full SKAdNetwork attribution information when a person clicks the ad:

`{itunes_item_id}`  
The App Store ID of the app that the ad impression advertises.

`attributionDestination`  
The effective top-level domain and one more preceding domain component (eTLD+1) representation of the ad network that seeks ad attribution. This value needs to match the `source_domain` value in the request and response for Get a Signed Web Ad Impression Payload.

`attributionSourceNonce`  
A Base64URL-encoded representation of a one-time UUID value that you generate for each ad impression.

The `attributionSourceNonce` in a web ad link, the `source_nonce` in an AdImpressionRequest, and the `nonce` in an AdImpressionResponse all represent the same UUID, but the encoding varies.

To generate an `attributionSourceNonce` for a web ad, Base64URL-encode the raw bytes of the UUID. Don’t encode a string representation of the UUID or lowercase the encoded UUID. The device uses the same encoding as `attributionSourceNonce` for the `source_nonce` value in the AdImpressionRequest. However, you use the dash-separated string representation of the UUID for the `nonce` value in an AdImpressionResponse.

### Use the link in a web ad

Add the link to an advertisement or an app promotion on the webpage where you want people to encounter it. You can cover the entire advertisement with the link or include it as a pure hyperlink to the App Store.

### Implement the signed web ad impression endpoint

When a person clicks the web ad, their device generates an AdImpressionRequest using the information from the web ad link. The device then sends a request to the Get a Signed Web Ad Impression Payload endpoint with the ad-impression request in the request body.

Important

The device doesn’t follow an HTTP redirect when it sends the request to the Get a Signed Web Ad Impression Payload endpoint at the `attributionDestination` URL.

On your server, implement the Get a Signed Web Ad Impression Payload endpoint to return an AdImpressionResponse. For an example of the response format, see AdImpressionResponse.

For more information about generating the signature in your response, see Generating a signature for attributable web ads.

