

- SiriKit Cloud Media
-  Configure Your Service Endpoints 

Web Service Endpoint

# Configure Your Service Endpoints

Provide configuration details for your media server’s endpoints to a HomePod speaker or an Apple TV.

SiriKit Cloud Media 1.0.2+

## URL

``` source
GET https://cloudextension-testservice.local/api/configuration
```

## Header Parameters

`Accept-Language`

`string`

 (Required) 

The client’s current user interface language. Your service responds to requests with localized content for this language, if available.

`Cache-Control`

`string`

 (Required) 

Directives for your service’s caching behavior.

`If-None-Match`

ExtensionConfigTag

The identifier of the client’s current configuration information.

Maximum length: `1002`

`Request-Timeout`

`uint32`

 (Required) 

An approximate deadline, in seconds, for processing this real-time user request.

Minimum: `1`

`User-Agent`

`string`

 (Required) 

The extension protocol running on the client. This is an RFC 7231-compliant string that contains the product name *AppleCloudExtension* and the SiriKit Extension library version running on the client.

Maximum length: `250`

Value: `/AppleCloudExtension/([0-9]+\.[0-9]+\.[0-9]+) *.*/`

`x-applecloudextension-retry-count`

`uint32`

The number of previous requests from the client. The client omits this header on the first attempt.

Minimum: `1`

`x-applecloudextension-session-id`

`string`

 (Required) 

A constant session identifier to include in each request and response. Your service responds to each request with the session ID provided by the client.

Minimum length: `1`

Maximum length: `128`

## Response Codes

` 200 ``OK`

ExtensionConfig

`OK`

The request is successful.

Content-Type: application/jose

` 304 ``Not Modified`

`Not Modified`

The request’s ExtensionConfigTag indicates the client already has the current configuration.

## Discussion

You must cryptographically sign your configuration endpoint response in JSON Web Signature (JWS) format when communicating with the SiriKit Cloud Media API via Media Setup. JWS is part of the JSON Object Signing and Encryption (JOSE) open standard (RFC 7515) that defines a way to cryptographically sign transmitted data.

To generate a signed JWS:

- Create the JWS header.

- Create the JWS payload.

- Sign the JWS.

To create a JWS to communicate with the SiriKit Cloud Media API, use the following fields and values in the header:

| Header | Description |
|----|----|
| `alg` | The algorithm used to sign the JWS. For SiriKit Cloud Media, use `ES256`. |
| `kid` | Your app bundle identifier registered for the service. |
| `typ` | The type used by the complete JWS. For SiriKit Cloud Media, use `JOSE`. |
| `cty` | The content type used by the payload of the JWS. For SiriKit Cloud Media, use `JSON`. |

The JWS payload contains JSON-encoded information specific to the SiriKit Cloud Media API and your app, such as intent type, media queues, base URLs for endpoints, and supported API version. The format is defined in the SiriKit Cloud Media OpenAPI Specification. Here are the major keys in the configuration data:

| Key | Description |
|----|----|
| `intent` | **(Required)** This is a mapping of (abbreviated) Intent names to the SiriKit Cloud Media endpoints and configuration options supported by web endpoint handlers. |
| `media` | **(Required)** This is a mapping of queue API endpoints for the particular configuration valid for the service (or user). |
| `url` | The base URL for endpoints. This value can be a fully qualified URL, or a relative URL, used to retrieve this configuration resource. |
| `version` | **(Required)** The supported version of the SiriKit Cloud Media API. |

After creating the JWS, sign it using the Elliptic Curve Digital Signature Algorithm (ECDSA) with the P-256 curve and the SHA-256 hash algorithm. The SiriKit Cloud Media API identifies the intents and media endpoints your service supports by parsing the configuration response. In the decoded JWS below, the service is configured to support the add media, play media, and update media affinity intents, and provides URLs to each as well as the media queue endpoints used to handle intent responses:

```
```

Regardless of the programming language you’re using with the SiriKit Cloud Media API, there are a variety of open source libraries available online for creating and signing JWS data. Please verify and validate your response before sending it to the SiriKit Cloud Media API.

## See Also

### Device Configuration

type ExtensionConfigTag

A unique identifier for a specific media service configuration.

object ExtensionConfig

Instructions for accessing your media service’s endpoints.

object PlayMediaControlActivity

Options for reporting playback progress.

