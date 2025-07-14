

- Apple News
- Apple News API
-  About the Apple News Security Model 

Article

# About the Apple News Security Model

Learn how the Apple News API authenticates clients, authorizes your news channel, and enforces confidentiality.

## Overview

Security is the highest priority of the Apple News API, and it conforms to these principles:

- Authentication: Validates the identity of the client.

- Authorization: Provides fine-grained control over clients, allowing only specific actions that the client has permission to perform.

- Confidentiality: Protects information by encrypting data that’s exchanged between client and server.

Note

In this documentation, a *client* is a remote system identified by an API key. News Publisher provides you with the API key when you set up your channel. See Use your CMS with News Publisher.

### Authentication

The Apple News API authenticates clients using message authentication codes (MAC) — specifically, hash-based message authentication codes (HMAC).

MAC/HMAC is a common authentication mechanism for REST APIs and provides a way for a server to prove to its client that it possesses a particular shared secret.

The server uses the following MAC/HMAC authentication process:

- The client uses the cryptographic hash function SHA-256 to combine the secret and the content of the message to generate a cryptographic hash.

- The server uses the same secret and message content to generate the server-side cryptographic hash.

- The server verifies the hash the client provides to check if it matches the serverʼs hash.

- If the hash the client provides doesn’t match the server’s hash, the client might not have the correct secret, the client might have generated the hash incorrectly, or someone may have tampered with the message.

For more information, see Authenticating the Apple News API.

### Authorization

The Apple News API enforces authorization by tying each API key to a single channel. A client thatʼs using a particular API key can create, read, update, or delete only those resources that are owned by the channel.

The Apple News API doesn’t support roles. Every key for a particular channel has access to all API endpoints for that channel.

### Confidentiality

Transport layer security (TLS) enforces confidentiality in the Apple News API. The Apple News API listens for requests served over TLS/HTTPS only. This ensures that all requests and responses are fully encrypted.

### Authenticating the Apple News API

To meet the authentication requirements of the Apple News API, follow these steps for each request.

#### Create a Request

If the request is a `GET`, create a canonical request by using a byte-wise concatenation of the following:

- The `HTTP` method (for example, `GET` or `POST` in all caps)

- The full `URL` of the request

- The current date in ISO 8601 format

Note

Comscore analytics require a canonical URL for data collection and reporting.

If the request is a `POST` request with an entity, then include the following in the canonical request:

- The value of the `Content-Type` header

- The full content of the entity

#### Complete the Request

1.  Decode the secret that you received as a Base64-encoded string when you created your channel in News Publisher.

2.  Use HMAC SHA-256 to generate a hash out of the canonical request you created in Create a Request.

3.  Encode the hash with Base64.

4.  Set the Authorization header as follows, then send the request:

```
HHMAC; key=; signature=; date=
```

where `` is the date string you created in Create a Request.

For more information about authenticating the Apple News API, see Apple News API Tutorial.

## See Also

### Essentials

Getting Ready to Publish and Manage Your Articles

Get set up for using the Apple News API.

About Apple News API Field Types

Understand the standard field types used in the Apple News API.

Formatting Strings

Learn how to format strings to pass to the API client.

