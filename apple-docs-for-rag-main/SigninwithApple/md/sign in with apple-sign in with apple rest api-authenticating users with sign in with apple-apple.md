

- Sign in with Apple
- Sign in with Apple REST API
-  Authenticating users with Sign in with Apple 

Article

# Authenticating users with Sign in with Apple

Securely authenticate users and create accounts for them in your app.

## Overview

Sign in with Apple lets users log in to your app across all of your platforms using their two-factor authentication Apple ID. After the user chooses to use Sign in with Apple to log in, your app receives tokens and user information that you can verify from a server.

When the user attempts to sign in using Sign in with Apple, the sequence in the following diagram begins:

You may group apps in your developer account for Sign in with Apple so an app only requests information the first time the user logs in. A simple confirmation to continue appears even if the app bundle IDs are different across systems, such as iOS, macOS, and the web.

### Authenticate the user and request information

Initialize an authentication session with your app server and associate a client session with an ID token using the `nonce` value. You can request to receive the user’s information, such as name and email address. If the user approves accessing this information, your authorization request includes the requested information.

Sign in with Apple protects user accounts by using two-factor authentication. Users that log in to an Apple device can quickly sign in to your app in the following ways:

- With Face ID or Touch ID on passcode-protected devices

- With a passcode, if Touch ID or Face ID isn’t available

- With an Apple ID password, if the passcode isn’t set

Native apps only allow the signed-in iCloud user to use Sign in with Apple. Web-based interactions allow logins using any Apple ID.

Note

On non-Apple devices, users must log in with their Apple ID, password, and two-factor authentication code.

Apple determines whether a user is a real person by combining on-device machine learning, account history, and hardware attestation using privacy-preserving mechanisms. There are three possible values when determining whether a user is a real person:

`2` (or `LikelyReal`)  
The user appears to be a real person, and you can treat this account as a valid user. You can skip any additional fraud verification checks or CAPTCHAs that your app normally uses. For more information, see ASUserDetectionStatus.likelyReal.

`1` (or `Unknown`)  
The system can’t determine whether the user is a real person. The server may return this value if status determination takes too long. Treat this user as any other account with limited information that requires additional verification steps. Don’t block service, because the user may be a real person. For more information, see ASUserDetectionStatus.unknown.

`0` (or `Unsupported`)  
Real user status is only available in iOS 14 and later, macOS 11 and later, watchOS 7 and later, and tvOS 14 and later. Previous versions of iOS, macOS, watchOS, tvOS return `Unsupported`. For more information, see ASUserDetectionStatus.unsupported.

This system for detecting whether the user is real is tuned for high-precision and moderate recall time. You may also use it as a feature in your own machine-learning models for detecting account fraud.

When someone uses your app and Sign in with Apple for the first time, the identification servers return the user status. Subsequent attempts don’t return the user status.

After the user logs in to your app using Sign in with Apple on one of their devices, they can sign in on all of their devices. Deleting your app from a device doesn’t affect this capability. If the user reinstalls your app, they can continue to use Sign in with Apple on any of their devices to sign in with their existing account.

### Retrieve the user’s information from Apple ID servers

The information you retrieve must include the credentials required to verify the user’s identity. The server returns the credentials and user information based on the initial request. The information that returns can include user identity, full name, verified email address, and real user status.

After successfully authenticating the user, the server returns an identity token, authorization code, and user identifier to your app.

The identity token is a JSON Web Token (JWT) and contains the following claims:

`iss`  
The issuer registered claim identifies the principal that issues the identity token. Because Apple generates the token, the value is `https://appleid.apple.com`.

`sub`  
The subject registered claim identifies the principal that’s the subject of the identity token. Because this token is for your app, the value is the unique identifier for the user.

`aud`  
The audience registered claim identifies the recipient of the identity token. Because the token is for your app, the value is the `client_id` from your developer account.

`iat`  
The issued at registered claim indicates the time that Apple issues the identity token, in the number of seconds since the Unix epoch in UTC.

`exp`  
The expiration time registered claim identifies the time that the identity token expires, in the number of seconds since the Unix epoch in UTC. The value must be greater than the current date and time when verifying the token.

`nonce`  
A string for associating a client session with the identity token. This value mitigates replay attacks and is present only if you pass it in the authorization request.

`nonce_supported`  
A Boolean value that indicates whether the transaction is on a nonce-supported platform. If you send a nonce in the authorization request, but don’t see the nonce claim in the identity token, check this claim to determine how to proceed. If this claim returns true, treat nonce as mandatory and fail the transaction; otherwise, you can proceed treating the nonce as optional.

`email`  
A string value that represents the user’s email address. The email address is either the user’s real email address or the proxy address, depending on their private email relay service. This value may be empty for Sign in with Apple at Work & School users. For example, younger students may not have an email address.

`email_verified`  
A string or Boolean value that indicates whether the service verifies the email. The value can either be a string (`"true" or "false"`) or a Boolean (`true` or `false`). The system may not verify email addresses for Sign in with Apple at Work & School users, and this claim is `"false"` or `false` for those users.

`is_private_email`  
A string or Boolean value that indicates whether the email that the user shares is the proxy address. The value can either be a string (`"true"` or `"false"`) or a Boolean (`true` or `false`).

`real_user_status`  
An Integer value that indicates whether the user appears to be a real person. Use the value of this claim to mitigate fraud. The possible values are: `0` (or `Unsupported`), `1` (or `Unknown`), `2` (or `LikelyReal`). For more information, see ASUserDetectionStatus. This claim is present only in iOS 14 and later, macOS 11 and later, watchOS 7 and later, tvOS 14 and later. The claim isn’t present or supported for web-based apps.

`transfer_sub`  
A string value that represents the transfer identifier for migrating users to your team. This claim is present only during the 60-day transfer period after you transfer an app. For more information, see Bringing new apps and users into your team.

Note

If the user signs in with a managed Apple ID, the value of the `email` claim is a real email address, not a proxy address. Alternatively, if the managed Apple ID is in Apple School Manager, the `email` claim may be empty. Students, for example, often don’t have an email that the school issues.

Use the authorization code to verify the token claims with Apple servers, and exchange them for refresh tokens. For more information, see Generate and validate tokens.

The user identifier has the following characteristics:

- Consists of a unique, stable string, and serves as the primary identifier of the user

- Uses the same identifier across all of the apps in the development team associated with your Apple Developer account

- Differs for the same user across different development teams, and can’t identify a user across development teams

- Doesn’t change if the user stops using Sign in with Apple with your app and later starts using it again

- Typically stores alongside the user’s primary key in your database

Use the user identifier instead of an email address to identify the user. If you request the user’s full name, Sign in with Apple collects the information to pass along to your app. The name defaults to the user’s name from their Apple ID, but the user can change their name.

Important

Apple doesn’t receive the user’s full name shared with the system UI. The raw data is passed directly to your app from the browser and is not included in the user’s identity token. To help prevent cross-site scripting attacks, validate and sanitize the user-submitted first and last name values before storing on your app servers.

If you request the user’s verified email address, Sign in with Apple prompts the user to share it with your app. The user may choose to share their real email address or an anonymous one that uses the private email relay service. In both cases, Apple verifies that the email address works and is ready for use.

For more information, see Communicating using the private email relay service.

### Send information to app servers and verify tokens

Ensure that your app relays the credentials and user information to your app servers. The API collects this information and shares it with your app the first time the user logs in using Sign in with Apple. If the user then uses Sign in with Apple on another device, the API doesn’t ask for the user’s name or email again. It collects the information again only if the user stops using Sign in with Apple and later reconnects to your app.

Although Apple provides the user’s email address in the identity token on all subsequent API responses, it doesn’t include other information about the user, such as their name. When you receive user information from the API response, immediately store it locally so your app can access it again in the event of a process or network failure.

Your app servers verify the validity of the token credentials with Apple ID servers. For more information, see Verifying a user.

### Prevent duplicate accounts

A user may already have an account in your system, but may attempt to use Sign in with Apple to log in to that account. Sharing the real email address that’s associated with the user’s Apple ID may not help because it may not be the same email the user uses to create the account with your system. There are a couple of ways you can mitigate this issue:

- Implement the ASAuthorizationPasswordProvider class to detect and offer keychain credentials that the system already knows about. This works seamlessly to detect and use existing accounts, and prevents creating new accounts using Sign in with Apple.

- For new accounts that use Sign in with Apple, let the user know that they’re creating a new account, and ask if they have any existing accounts to link to.

## See Also

### Authentication and verification of users

Verifying a user

Check the validity and integrity of a user’s identity token.

