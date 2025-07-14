

- Security
-  Shared Web Credentials 

API Collection

# Shared Web Credentials

Share credentials between iOS apps and their website counterparts.

## Overview

The `Security.SecSharedCredentials` API provides functions for storing and requesting shared password-based credentials. Users often save their username and password in their iCloud keychain when logging into websites in Safari. Later, they may run a native app from the same developer to access the same account. With shared web credentials, the app can access the credentials stored for the website instead of requiring the user to reenter a username and password. Users can also create new accounts, update passwords, or delete their accounts from within the app. These changes are then saved and used by Safari.

Note

Accessing shared web credentials requires permission from the app, the website, and the user.

## Topics

### First Steps

Supporting associated domains

Connect your app and a website to provide both a native app and a browser experience.

Managing Shared Credentials

Use shared web credentials to create a seamless experience for the user.

### Password Sharing

func SecAddSharedWebCredential(CFString, CFString, CFString?, (CFError?) -> Void)

Asynchronously stores (or updates) a shared password for a website.

func SecRequestSharedWebCredential(CFString?, CFString?, (CFArray?, CFError?) -> Void)

Asynchronously obtains one or more shared passwords for a website.

Deprecated

func SecCreateSharedWebCredentialPassword() -> CFString?

Returns a randomly generated password.

let kSecSharedPassword: CFString

A dictionary key whose value is the shared password.

