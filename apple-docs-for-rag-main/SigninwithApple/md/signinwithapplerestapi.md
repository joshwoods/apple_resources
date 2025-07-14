

Framework

# Sign in with Apple REST API

Communicate between your app servers and Apple’s authentication servers.

## Overview

The Sign in with Apple REST API is a web service that connects you to Apple’s authentication servers. Use this service to generate and validate the identity tokens used to verify a user’s identity.

To sign in from a web app or other platform, like Android, use Sign in with Apple JS. Alternatively, to let users set up accounts and sign in to your native iOS, macOS, tvOS, and watchOS apps, use the Authentication Services framework.

## Topics

### Authentication and verification of users

Authenticating users with Sign in with Apple

Securely authenticate users and create accounts for them in your app.

Verifying a user

Check the validity and integrity of a user’s identity token.

### Generating and revoking tokens

Creating a client secret

Generate a signed token to identify your client application.

Fetch Apple’s public key for verifying token signature

Fetch Apple’s public key to verify the ID token signature.

Generate and validate tokens

Validate an authorization grant code delivered to your app to obtain tokens, or validate an existing refresh token.

Revoke tokens

Invalidate the tokens and associated user authorizations for a user when they are no longer associated with your app.

### Common objects

object JWKSet

A set of JSON Web Key objects.

object TokenResponse

The response token object returned on a successful request.

object ErrorResponse

The error object returned after an unsuccessful request.

### Endpoints

Get a Sign in with Apple button that contains just the Apple logo.

Get a Sign in with Apple button that is center-aligned.

Get a Sign in with Apple button that is left-aligned.

Request an authorization to the Sign in with Apple server

Add a Sign in with Apple authorization flow to apps and web services that can’t directly access Sign in with Apple JS.

## See Also

### Web support

Sign in with Apple JS

Provide users a fast, secure way to sign in to your web service with their Apple ID.

