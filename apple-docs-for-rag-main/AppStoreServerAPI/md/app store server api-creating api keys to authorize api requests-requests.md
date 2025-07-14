

- App Store Server API
-  Creating API keys to authorize API requests 

Article

# Creating API keys to authorize API requests

Create API keys you use to sign JSON Web Tokens and authorize API requests.

## Overview

The App Store Server API and External Purchase Server API require JSON Web Tokens (JWTs) to authorize each request you make to the API. You generate JWTs using a private API key that you download from App Store Connect. For information about generating the JWT using your private key, see Generating JSON Web Tokens for API requests.

An API key has two parts: a public portion that Apple keeps, and a private key that you download. Use the private key to sign tokens that authorize the API to access or submit your data to the App Store.

Important

Store your private keys in a secure place. Don’t share your keys, don’t store keys in a code repository, and don’t include keys in client-side code. If you suspect a private key is compromised, immediately revoke the key in App Store Connect. See Revoking API Keys for details.

Use the API key for the App Store Server API and the External Purchase Server API. You can’t use the key for other Apple services.

### Generate a private key

To generate keys, you must have an Admin role or Account Holder role in App Store Connect. You may generate multiple API keys. To generate an API key to use with the App Store Server API and External Purchase Server API, log in to App Store Connect and complete the following steps:

1.  Select Users and Access, and then select the Keys tab.

2.  Select In-App Purchase under the Key Type.

3.  Click Generate API Key or the Add (+) button.

4.  Enter a name for the key. The name is for your reference only and isn’t part of the key itself.

5.  Click Generate.

The new key’s name, key ID, a download link, and other information appears on the page.

### Download and store the private key

After generating your API key, App Store Connect gives you the opportunity to download the private half of the key. The private key is only available for download a single time.

1.  Log in to App Store Connect.

2.  Select Users and Access, and then select the Keys tab.

3.  Select In-App Purchase under the Key Type.

4.  Click Download API Key next to the new API key.

The download link appears only if you haven’t yet downloaded the private key. Apple doesn’t keep a copy of the private key. Store your private key in a secure place.

## See Also

### Essentials

Simplifying your implementation by using the App Store Server Library

Use Apple’s open source library to create JSON Web Tokens (JWT) to authorize your calls, verify transactions, extract transaction identifiers from receipts, and more.

Generating JSON Web Tokens for API requests

Create JSON Web Tokens signed with your private key to authorize requests for App Store Server API and External Purchase Server API.

Identifying rate limits

Recognize the rate limits that apply to App Store Server API endpoints and handle them in your code.

App Store Server API changelog

Learn about new features and updates in the App Store Server API.

