

- Sign in with Apple
-  Processing changes for Sign in with Apple accounts 

Article

# Processing changes for Sign in with Apple accounts

Manage user-initiated modifications to maintain privacy with server-to-server notifications.

## Overview

Sign in with Apple users can modify their accounts, including deleting or disabling their Apple IDs. If your app or website hosts such an account, Apple can alert you when these changes occur by delivering developer notifications to your server. To learn how your users manage their account preferences for your app, see Manage the apps that you use with Sign in with Apple.

### Set up your server

To receive server notifications for Sign in with Apple, your server must support the Transport Layer Security (TLS) 1.2 protocol or later. When determining the endpoint URL on your server to receive notifications, you may use the same URL for multiple developer teams and apps. To configure your Sign in with Apple service to receive notifications, see Enabling server-to-server notifications.

### Decode and validate the notifications

These notifications contain a cryptographically signed payload, in JSON Web Signature (JWS) format, signed by Apple’s private key. After your server receives a notification, examine the JWS payload and use the algorithm specified in the header’s `alg` parameter to validate the signature. For more information, see Fetch Apple’s public key for verifying token signature.

After validating the token signature, your server performs work according to the `type` value in the `events` claim of the token. The notification payload object contains information about user-initiated account modification events. The event types include the following:

`email-disabled`  
The user disables email forwarding to their personal email address using Hide My Email.

email-enabled  
The user enables email forwarding to their personal email address using Hide My Email.

`consent-revoked`  
The user revokes consent for your app to use their Apple ID and their credentials become invalid.

`account-delete`  
The user requests that Apple permanently delete their Apple ID.

Expect an HTTP POST response similar to the following example:

```
HTTP/1.1 200 OK
Content-Type: application/json;charset=UTF-8
Cache-Control: no-store
Pragma: no-cache

{
    "payload": ""
}
```

### Process a user’s email forwarding change

Users can enable or disable email forwarding to your app or website. When a user enables email forwarding, Apple sends a JWT to your registered endpoint URL with the `type` value of `email-enabled` in the `events` claim. A decoded payload for an email-enabled notification has the following format:

```
```

When a user disables email forwarding, Apple sends a JWT to your registered endpoint URL with the `type` value of `email-disabled` in the `events` claim. A decoded payload for an email-disabled notification has the following format:

```
```

To allow or prevent sending emails to the email address, be sure to update your server’s records according to your process. For more information, see Communicating using the private email relay service.

### Process disabling and deleting a user’s Apple ID

Users can disable their Apple ID for a specific primary app ID, or delete their Apple ID account entirely. When a user disables their Apple ID for an app or app group, Apple sends a JWT to your registered endpoint URL with the `type` value of `consent-revoked` in the `events` claim. A decoded payload for a consent-revoked notification has the following format:

```
```

When a user requests for Apple to permanently delete their Apple ID, Apple sends a JWT to your registered endpoint URL with the `type` value of `account-delete` in the `events` claim. A decoded payload for an account-delete notification has the following format:

```
```

Important

When a user permanently deletes their Apple ID, Sign in with Apple invalidates all user tokens and disables email forwarding for all associated apps. For native apps, the system doesn’t send a credentialRevokedNotification. Use getCredentialState(forUserID:completion:) to respond to account deletion events.

To indicate when the user disables or permanently deletes their Apple ID, be sure to update your server’s records according to your process.

## See Also

### Web support

Displaying Sign in with Apple buttons on the web

Configure the appearance of Sign in with Apple buttons with CSS styles.

Configuring your environment for Sign in with Apple

Authenticate users with your web service by associating an existing app with a Services ID and private key.

