

- iWork Document Exporting API
-  Export a PDF document from an iWork file 

Web Endpoint

# Export a PDF document from an iWork file

Create a PDF preview of an iWork document using JSON Web Token (JWT) authorization.

iWork 14.0+

## URL

``` source
POST https://iworkpreviewapi.icloud.com/iwork/api/v2/export
```

## Header Parameters

`Content-Length`

`int64`

 (Required) 

The number of bytes in the request body as defined in RFC 7230.

The service doesn’t support chunked transfer coding.

`authorization`

`string`

 (Required) 

A JWT as defined in the Authentication and as defined in the Authentication and request payload section, below.

## HTTP Body

`binary`

The body of the request. The body contains the iWork document for the service to export in raw binary form. If the original file is a package file, zip it before adding to the request.

Content-Type: application/octet-stream

## Response Codes

` 200 ``OK`

`binary`

`OK`

Successful export.

If the service successfully processed the request and exported the document, the server returns an HTTP 200 response with the exported file in the body.

Content-Type: application/octet-stream

` 400 ``Bad Request`

`string`

`Bad Request`

Invalid request.

If the request is invalid for some reason (such as missing or invalid header values), the server returns an HTTP 400 response.

The server returns the reason for the error in the response body, for example: `Invalid filename`.

Content-Type: text/plain

` 403 ``Forbidden`

`string`

`Forbidden`

Authentication failure.

If the server can’t validate the signature, either because the signature is invalid, or because the key pair can’t recognize the signature, the server returns an HTTP 403 response with body `Invalid signature`.

If the document is password-protected, the server responds with a HTTP 403 response with body `Password protected document`.

Content-Type: text/plain

` 404 ``Not Found`

`string`

`Not Found`

Content-Type: text/plain

` 411 ``Length Required`

`string`

`Length Required`

Content-Type: text/plain

` 413 ``Request Entity Too Large`

`string`

`Request Entity Too Large`

Request too large.

The server returns this error if the document is over 1 GB.

Content-Type: text/plain

` 429 `

`string`

Client is sending too many requests.

If you’re sending too many requests, the server returns an HTTP 429 response. The server may give this response without completely reading the contents of the request. In this case, don’t retry the request.

Content-Type: text/plain

` 500 ``Internal Server Error`

`string`

`Internal Server Error`

For other errors, the server returns an HTTP 500 response.

For export errors caused by a corrupted document or other irrecoverable errors, the response body contains `Irrecoverable export error`. In this case, don’t retry exporting the same document. In general, don’t retry unless there is a `Retry-After` header in the response.

Content-Type: text/plain

` 503 ``Service Unavailable`

`string`

`Service Unavailable`

Server asks client to retry.

In some situations where the server is under heavy load, the server may return an HTTP 503 response. The `Retry-After` response header specifies the number of seconds after which you may retry. Don’t retry unless there is a `Retry-After` header. The server may give this response without completely reading the contents of the request.

Content-Type: text/plain

## Privacy Notice

It’s important for apps to inform people that uploaded iWork documents are temporarily stored on Apple servers for the purpose of conversion. Provide people the option to enable and disable the iWork preview feature, and display a privacy notice when doing so, such as “When using iWork online previews, your files will be temporarily stored on Apple servers.”

## Supported files

The maximum file size the service supports is 1 GB and the service can only convert documents not protected with a password.

## Authentication and request payload

For each request, the iWork service requires a signature so that the service can confirm that the client has permission to access the API. The service uses a JSON Web Token (JWT) to transfer the signature, information about the client and the details of the document export request. Sign the JWT with an ES256 key acquired from Apple Developer Keys.

Using Open Source libraries recommended by JWT.io may simplify the process of constructing and signing JWTs.

Include these claims in the JWT header:

| Header claims | Value |
|----|----|
| `alg` | The name of the algorithm used to sign the token. The algorithm the service supports is “ES256”. |
| `kid` | The ID of the Apple Developer Key used to sign the token. The portal displays this ID on the key download page when downloading the key from Apple developer portal. |

Include these claims in the JWT payload:

| Payload claims | Value |
|----|----|
| `iss` | Issuer of the token. This is the ID of the Apple Developer Team, your team’s ID, displayed in the membership details section of the Apple developer portal. |
| `encoded_filename` | The original filename of the file, encoding in UTF-8 and then encoded in URL-safe base64. If the name is too long, or if it contains invalid characters, the service may ignore parts of the filename. |
| `export_format` | The format to export. Currently, the service only supports `com.adobe.pdf`. |
| `iat` | The creation time of the token, in terms of the number of seconds since the epoch, in UTC. |
| `exp` | Optional. The time at which the token expires, in terms of the number of seconds since the epoch, in UTC. If you don’t provide an expiration time, the default value is four hours from the time specified by `iat`. The actual expiry would be the specified value or four hours, whichever is smaller. |

Put the signed JWT as-is in the HTTP `authorization` header.

Clients need to ensure that their system clocks are accurate: The service rejects the signed JWT if the current time falls outside of the time window specified by `iat` and `exp`. Reconstruct and sign the JWT with a new `DateTime` for each request even if you’re retrying the request.

The method to authenticate and sign the requests may change in light of new developments in the security field. Apple will give notice to parties using the API if and when this happens.

## Examples

### Export Request

The following example demonstrates an export request using the headers and their associated values you pass to the API:

```
POST /iwork/api/v2/export HTTP/1.1
authorization: eyJhbGciOiJFUzI1NiIsImtpZCI6IkIzQ1U3TUhQUzgifQ.eyJlbmNvZGVkX2ZpbGVuYW1lIjoiOEorWWdDQmpiRzkxWk9LWWdTNXVkVzFpWlhKeiIsImV4cG9ydF9mb3JtYXQiOiJjb20uYWRvYmUucGRmIiwiaWF0IjoxNjkzMDA0MDQxLCJpc3MiOiI0M0tUTFlYTTRHIiwiZXhwIjoxNjkzMDExMjQxfQ.4Uw6_WeYZgmi2gXC82tBeSXDGwa2ajouG2tQVgNlWPld0mxTHuc0VSNWDUOr5QlPZqjJYMKEdZ4wpTmEfuuVcg
Content-Type: application/octet-stream
Host: https://iworkpreviewapi.icloud.com
Content-Length: 323927

```

The filename is “😀 cloud☁.numbers”.

### Generating a JWT using JSON Object Signing and Encryption (JOSE)

For more information on the JOSE NodeJS package, see the JOSE package documentation.

```
```

Using the above Apple Developer key, this is the JWT header and payload the package signs:

```
```

And the resulting signed JWT is:

`eyJhbGciOiJFUzI1NiIsImtpZCI6IkhCTFVGRFkzNjcifQ.eyJlbmNvZGVkX2ZpbGVuYW1lIjoiOEorWWdDQmpiRzkxWk9LWWdTNXVkVzFpWlhKeiIsImV4cG9ydF9mb3JtYXQiOiJjb20uYWRvYmUucGRmIiwiaWF0IjoxNjkzMDA1MDkyLCJpc3MiOiI0M0tUTFlYTTRHIiwiZXhwIjoxNjkzMDEyMjkyfQ.o4haQp-Fo-r_-_rELXhMEbOIXU8n-mr8sAogH8b6i8x9_VdHYnTw29r7hu0OjwA_HWNWfwpBvgLNtqr2dcl4Vg`

Note

The signed JWT can be different for the same input.

