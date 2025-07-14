

- Sign in with Apple
- Sign in with Apple REST API
-  Verifying a user 

Article

# Verifying a user

Check the validity and integrity of a user’s identity token.

## Overview

After your app receives a user’s information, you can verify their associated identity token with the server to confirm that the token isn’t expired and ensure it hasn’t been tampered with or replayed to your app. For information about retrieving the identity token, see Authenticating users with Sign in with Apple.

### Verify the identity token

Start by securely transmitting the identity token and authorization code to your app server. For more about the information required to verify a user’s identity, see Authenticating users with Sign in with Apple.

Note

To obtain the identity token from their server, web apps must validate the authorization code using the Generate and validate tokens endpoint.

To verify the identity token, your app server must:

- Verify the JWS E256 signature using the server’s public key

- Verify the `nonce` for the authentication

- Verify that the `iss` field contains `https://appleid.apple.com`

- Verify that the `aud` field is the developer’s `client_id`

- Verify that the time is earlier than the `exp` value of the token

### Obtain a refresh token

After verifying the identity token on your server, call the Generate and validate tokens endpoint with the `client_id`, `client_secret`, and `nonce` information.

On success, the server issues a refresh token, which you use to obtain access tokens with future calls. You may verify the refresh token up to once a day to confirm that the user’s Apple ID on that device is still in good standing with Apple’s servers. Apple’s servers may throttle your call if you attempt to verify a user’s Apple ID more than once a day.

You may continue to use the same refresh token until it’s invalidated — for example, by an Apple ID account password change, or when a user revokes access to your app — or the token verification fails. If any step of the token verification fails, direct your app to fetch a new identity token for the user. Obtaining a new identity token on the device requires user interaction.

### Manage the user session

After verifying the identity token, your app is responsible for managing the user session. You may tie the session’s lifetime to successful getCredentialState(forUserID:completion:) calls on Apple devices. This is a local, inexpensive, nonnetwork call enabled by the Apple ID system that keeps the Apple ID state on a device in sync with Apple servers.

User interaction is required any time a new identity token is requested. User sessions are long-lived on device, so calling for a new identity token on every launch, or more frequently than once a day, can result in your request failing due to throttling.

If the user’s Apple ID changes in the system, calls to `getCredentialState(forUserID:completion:)` indicate that the user changed. Assume that a different user has signed in and log out the app’s currently known user.

For apps running on other systems, use the periodic successful verification of the refresh token to determine the lifetime of the user session.

## See Also

### Authentication and verification of users

Authenticating users with Sign in with Apple

Securely authenticate users and create accounts for them in your app.

