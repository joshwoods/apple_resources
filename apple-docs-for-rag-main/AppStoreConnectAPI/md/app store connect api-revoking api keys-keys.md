

- App Store Connect API
-  Revoking API Keys 

Article

# Revoking API Keys

Revoke unused, lost, or compromised private keys.

## Overview

Revoke an API key immediately if it becomes inactive, lost, or compromised. A revoked API key denies access to the App Store Connect API on your organization’s behalf.

Important

Once you revoke an API key, you can’t reinstate it. Revoked keys are displayed for 30 days on the API Keys page under the Revoked heading.

### Revoking Team Keys

To revoke a team API key, log in to App Store Connect with an Admin account.

1.  Select Users and Access, then select the Keys tab.

2.  Click Edit next to the list of Active keys.

3.  Select the API keys to revoke, and click Revoke Key.

4.  Click the Revoke button to confirm.

### Revoking Individual Keys

There are two ways to revoke an individual API key, depending on your role. Begin both methods by logging in to App Store Connect.

To revoke keys for another user, as an Admin:

1.  Select Users and Access, then select the Keys tab.

2.  Click Individual Keys.

3.  Click Edit next to the list of Active keys.

4.  Select the API keys to revoke, and click Revoke Key.

5.  Click the Revoke button to confirm.

To revoke your own key:

1.  Go to your user profile.

2.  Scroll down to Individual API Key.

3.  Click Revoke.

4.  Click the Revoke button to confirm.

Tip

Admins can prevent a user from creating an Individual Key by removing the Generate Individual API Keys permission.

## See Also

### Essentials

Creating API Keys for App Store Connect API

Create API keys to sign JSON Web Tokens (JWTs) and authorize API requests.

Generating Tokens for API Requests

Create JSON Web Tokens (JWTs) signed with your private key to authorize API requests.

Identifying Rate Limits

Recognize the rate limits that REST API responses provide and handle them in your code.

Uploading Assets to App Store Connect

Upload screenshots, app previews, attachments for App Review, and routing app coverage files to App Store Connect.

App Store Connect API Release Notes

Learn about new features and updates in the App Store Connect API.

