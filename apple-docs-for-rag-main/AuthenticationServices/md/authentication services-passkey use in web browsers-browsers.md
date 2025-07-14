

- Authentication Services
-  Passkey use in web browsers 

API Collection

# Passkey use in web browsers

Register and authenticate website users by using passkeys.

## Overview

If your browser app uses WKWebView to display web content, WebKit automatically handles `WebAuthentication` challenges in web pages and requests credentials from the person using the browser. If your browser app uses an alternative web browser engine—for example, an alternate browser engine for iPhone that you write using BrowserEngineKit—when the website makes a `WebAuthentication` challenge, use ASAuthorizationController to discover and use credentials to respond to the challenge. ASAuthorizationController works with passkeys stored on the keychain or managed by third-party credential managers.

The person using your browser chooses whether to let your app access their passkeys. Use ASAuthorizationWebBrowserPublicKeyCredentialManager to determine whether you browser app has access, and to request access if it has no access.

## Topics

### Website authorization

Authenticating people by using passkeys in browser apps

Provide a secure and convenient alternative to passwords.

class ASAuthorizationWebBrowserPublicKeyCredentialManager

A class that you use to request access to a person’s passkeys in a web browser, and that reports on the access status.

### Website authentication requests

protocol ASAuthorizationWebBrowserExternallyAuthenticatableRequest

An authorization request for which a web browser can retrieve credentials.

protocol ASAuthorizationWebBrowserPlatformPublicKeyCredentialAssertionRequest

An interface you use to respond to authentication challenges in a web browser.

protocol ASAuthorizationWebBrowserPlatformPublicKeyCredentialRegistrationRequest

An interface you use to respond to passkey-creation challenges in a web browser.

### Website credential providers

protocol ASAuthorizationWebBrowserPlatformPublicKeyCredentialProvider

A mechanism you use to provide public key credential requests to a browser app.

## See Also

### Passkeys

Public-Private Key Authentication

Register and authenticate users with passkeys and security keys, without using passwords.

Connecting to a service with passkeys

Allow users to sign in to a service without typing a password.

