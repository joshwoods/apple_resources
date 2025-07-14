

- Sign in with Apple
-  Bringing new apps and users into your team 

Article

# Bringing new apps and users into your team

Receive Sign in with Apple users and associated apps from another team.

## Overview

When acquiring an app from another team that uses Sign in with Apple, you follow a specific process to receive signed-in users from the sending team.

Coordinate with the sending team transferring their users and apps over to your team. Then accept transfer identifers for all of the migrating users, and exchange the transfer identifiers for team-scoped identifiers and private email addresses to complete the process.

### Obtain team-scoped identifiers

The identity token issued by Apple contains the transfer identifier in the `transfer_sub` claim for all migrated users who sign into your application after the transfer, as well as the team-scoped identifier. See Authenticating users with Sign in with Apple for more information.

Use the transfer identifier to correlate the Sign in with Apple user in the data records migrated from the previous owner. The identity token continues to include the transfer identifier, for up to 60 days from the transfer date.

For users who don’t sign in after the transfer, you must generate an access token and use it to obtain your team-scoped identifier. Generate the access token with your client credential and provide scope as `user.migration` using the following HTTP POST method.

```
```

The HTTP POST method includes the following parameters:

`grant_type`  
The type of grant requested. Set to `client_credentials` as there are no user credentials. Access the migration endpoint using the client application’s credentials.

`scope`  
The scope of the migration. Set to `user.migration` in order to exchange the identifier.

`client_id`  
The identifier (App ID or Services ID) for the transferred app. The identifier must not include your Team ID, to help mitigate the possibility of exposing sensitive data to the end user.

`client_secret`  
The client secret of the recipient team, represented as a JSON Web Token (JWT). The JWT payload should contain a `sub` claim that matches the transferred app’s bundle ID or associated Services ID. For more information on generating a client secret, see Creating a client secret.

Expect an HTTP POST response similar to the following example.

```
```

### Exchange identifiers

Use the access token to call the `userMigrationInfo` endpoint. Provide the transfer identifier of the user as input using the following HTTP POST method.

```
```

The HTTP POST method includes the following parameters:

`transfer_sub`  
The transfer identifier that you obtained from the sending team.

`client_id`  
The identifier (App ID or Services ID) for the transferred app. The identifier must not include your Team ID, to help mitigate the possibility of exposing sensitive data to the end user.

`client_secret`  
The client secret of the recipient team, represented as a JSON Web Token (JWT). The JWT payload should contain a `sub` claim that matches the transferred app’s bundle ID or associated Services ID. For more information on generating a client secret, see Creating a client secret.

Expect an HTTP POST response similar to the following example.

```
```

The HTTP POST response includes the following parameters:

`sub`  
The recipient team-scoped identifier for the user. This value is the same as the `sub` in the ID token issued during user sign-in.

`email`  
The private email address specific to the recipient team. This attribute returns only if the user utilized a private email address with the transferred application.

`is_private_email`  
A Boolean indicator specifying if the email address provided is the private mail relay address.

The user identifier and the private email address are specific to your team, and all of your applications share the same identifier for the user. Avoid exposing the user identifier to a different team to prevent correlation of a user across teams.

Once 60 days have passed after transfer acceptance, the ID token no longer includes the transfer identifier. Also, the server endpoint used to obtain the team-scoped identifiers becomes inactive.

### Regroup your apps

If the sending team ungrouped their apps, coordinate with the team to regroup the apps after the transfer completes. See Group Apps for Sign in with Apple for more information.

Note

The service identifiers for web applications don’t require ungrouping. They transfer over automatically when their primary app transfers.

### Confirm the transferred credential state

Your transferred application starts receiving ASAuthorizationAppleIDProvider.CredentialState.transferred when you call getCredentialState(forUserID:completion:). This status indicates that the user identifier currently in use is the one associated with the delivering team.

The following code silently performs a new authorization in the background, and delivers the new user identifier to the ASAuthorizationControllerDelegate delegate object. It doesn’t involve any user interaction.

```
```

Upon receiving ASAuthorizationAppleIDProvider.CredentialState.transferred, you can consider the current session approved.

## See Also

### Transfers across teams

Transferring your apps and users to another team

Migrate Sign in with Apple users to another team.

