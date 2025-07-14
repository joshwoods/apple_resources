

- SiriKit Cloud Media
-  Retrieve an Asset’s Content Protection Key 

Web Service Endpoint

# Retrieve an Asset’s Content Protection Key

Provide the content key for a specific protected asset.

SiriKit Cloud Media 1.0.2+

## URL

``` source
POST https://cloudextension-testservice.local/api/queues/contentProtectionKey
```

## Header Parameters

`Accept-Language`

`string`

The client’s current user interface language. If possible, respond with localized content for this language.

`User-Agent`

`string`

 (Required) 

The client’s extension protocol. This is an RFC 7231-compliant string that contains the product name `AppleCloudExtension` and the version of the SiriKit extension library that’s running on the client.

Maximum length: `250`

Value: `/AppleCloudExtension/([0-9]+\.[0-9]+\.[0-9]+) *.*/`

`x-applecloudextension-retry-count`

`uint32`

The number of previous requests from the client. The client omits this header on the first attempt.

Minimum: `1`

`x-applecloudextension-session-id`

`string`

 (Required) 

A session identifier to pair each request and response. Respond to requests with the value the client provides.

Minimum length: `1`

Maximum length: `128`

## HTTP Body

ContentProtectionKeyRequest

A JSON object that contains the encrypted key request and identifies the protected asset.

Content-Type: application/json

## Response Codes

` 200 ``OK`

ContentProtectionKeyResponse

`OK`

The request is successful.

Content-Type: application/json

` 204 ``No Content`

`No Content`

The service is unable to provide a content key for the specified `assetIdentifier`.

` 401 ``Unauthorized`

`Unauthorized`

The request requires authorization. The client can attempt to reauthorize and then retry the request.

` 410 ``Gone`

`Gone`

The request includes an expired UserActivity, which the service is unable to use to provide a content key.

## Discussion

If your service implements content protection, the client requests an item’s content protection key from this endpoint after each of the following events:

- The client receives the queue’s initial item.

- The client preloads each subsequent item in the queue.

- The user manually transitions to an item in the queue.

For more information on providing your service’s content protection configuration, see ExtensionConfig.Media.Queues.ContentProtectionKey.

## See Also

### Content Protection

object ContentProtectionKeyRequest

A request for an item’s content protection key.

object ContentProtectionKeyResponse

A response to a request for an item’s content protection key.

type ContentProtectionKeySystem

The content protection key systems that SiriKit Cloud Media supports.

