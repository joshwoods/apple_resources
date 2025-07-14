

- ManagedApp
-  Accessing provisioned secrets with identifiers 

Article

# Accessing provisioned secrets with identifiers

Specify the secrets your app requires for device management features, receive secrets from MDM servers and use secrets in your app.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

## Overview

Some device management features rely on *secrets*, that is, secure credentials provisioned by an administrator (MDM admin) for your app, such as passwords, certificates, and identities. Secrets can support:

- Automatically logging in a person

- Cryptographic signing

- Certificate pinning to improve trust evaluation of servers and signatures

Your app accesses secrets by their identifier using the framework supplied secret *provider* classes. Each provider offers a list of identifiers that catalogs all the currently available secrets, of a particular type, that an MDM admin provisions. You can access secrets using predefined identifiers, or identifiers that you add to your app’s configuration.

The provider’s list of identifiers is an AsyncSequence. If your app requires notification when the available secrets change, or if your app supports dynamic lists of secrets, iterate the sequence for the lifetime of the app using `for await`.

## Specify the secrets your app supports

To implement features with secrets, identify the provisions that you require from MDM admins. Publish a specification that details the requirements in a location accessible to MDM admins; for example, hosting it on your app website.

Note

If your app also defines a configuration specification for general information, you can add your secrets requirements to the same document. For more information about general configuration, see Specifying and decoding a configuration.

When an admin provisions secrets on their MDM server according to your specification, they use Device Management. The device’s operating system works with Device Management to ingest the secrets on the device. From the perspective of your app, ManagedApp receives the secrets automatically.

## Retrieve secrets using a known identifier

The framework defines a provider class for each type of secret:

- ManagedAppPasswordsProvider

- ManagedAppCertificatesProvider

- ManagedAppIdentitiesProvider

A provider contains:

- An accessor that returns secrets by ID

- A list of identifiers that contains all of the currently available secrets

The following code acquires a password using the password(withIdentifier:) accessor with a predefined identifier:

```
```

Another task that often uses known identifiers is responding to client certificate authentication challenges. The following example responds to a client certificate challenge within the URLSessionDelegate callback, and requests an identity using the ManagedAppIdentitiesProvider accessor:

```
```

Important

For security reasons, only request a secret from the framework when your app needs it immediately. This minimizes the amount of time that the secret is in your app’s memory. Avoid logging sensitive information such as passwords or private-key data.

## Retrieve secrets using the provider’s identifiers sequence

If your app needs a notification when the available secrets change, or if your app maintains dynamic lists of secrets, use the provider’s AsyncSequence. Use a `for await` construct on the provider’s `identifiers` property to listen for changes. The following example builds a list of available usernames by iterating the ManagedAppIdentitiesProvider sequence:

```
```

Note

Instead of predefining identifiers, you can add identifiers to your configuration specification so the identifiers are flexible and MDM admins can configure them. For more information, see Specifying and decoding a configuration.

## Access an identity for authentication or signing

To log someone in, an app needs to authenticate with a server. To acquire the person’s identity to authenticate, pass the person’s username as the identifier argument of the identity provider’s accessor, for example:

```
```

Alternatively, your app can use the identity for cryptographic signing. Because SecIdentity is in the Security framework, you can create a cryptographic signature using other Security framework API. The following code begins a signature by acquiring a reference to the identity’s private key:

```
```

The SecKey object is an opaque reference to the underlying private key data that’s in system memory. Don’t load actual private key data in your app’s memory unless absolutely necessary; for example, when using the SecKeyCopyExternalRepresentation(_:_:) function.

While choosing the signing algorithm, call SecKeyIsAlgorithmSupported(_:_:_:) to ensure the admin-provisioned key supports the algorithm:

```
```

To facilitate compatibility, document the algorithms and associated key types your app supports in your specification.

Finally, create the signature:

```
```

## See Also

### Secrets and identifiers

class ManagedAppCertificatesProvider

A class that provides certificates that an MDM admin provisions for a managed app or extension.

class ManagedAppIdentitiesProvider

A class that provides identities that an MDM admin provisions for a managed app or extension.

class ManagedAppPasswordsProvider

A class that provides passwords that an MDM admin provisions for a managed app or extension.

