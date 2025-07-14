

- Updates
-  AuthenticationServices updates 

Article

# AuthenticationServices updates

Learn about important changes to AuthenticationServices.

## Overview

Browse notable changes in Authentication Services.

## June 2024

### Passkeys

- Automatically upgrade someone’s password to a passkey after your app supplies a password to AutoFill if they’re eligible, while still retaining their password in case they need it. To do this, call createCredentialRegistrationRequest(clientData:name:userID:requestStyle:), passing ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest.RequestStyle.conditional for the `requestStyle` parameter.

- Use the `prf` WebAuthentication extension to generate a symmetric key from a passkey, which you use for encrypting and decrypting someone’s data. Each passkey generates its own symmetric keys, which you can retrieve any time a user signs in with that passkey, in apps or on the web.

### Credential providers

- Indicate to the system that your credential provider participates in OTP AutoFill by adding the key `ProvidesOneTimeCodes` with the value `true` to the `ASCredentialProviderExtensionCapabilities` dictionary in your app’s information property list. Implement provideCredentialWithoutUserInteraction(for:) and prepareInterfaceToProvideCredential(for:) to handle the ASOneTimeCodeCredentialRequest type. Use completeOneTimeCodeRequest(using:completionHandler:) to return the one time code to the system.

- Supply AutoFill for text in arbitrary text fields, for example to complete information about an account that someone manages in your credential provider, or AutoFill text in secure notes. Indicate to the system that your credential provider supplies AutoFill text by adding the key ProvidesTextToInsert with the value true to the `ASCredentialProviderExtensionCapabilities` dictionary in your app’s information property list, and implement prepareInterfaceForUserChoosingTextToInsert(). When the person chooses the text to AutoFill in your UI, call completeRequest(withTextToInsert:completionHandler:) to supply the text to the system.

- Use ASPasskeyCredentialExtensionInput to represent `largeBlob` and `prf` extension input data in a passkey credential request. Return output for these WebAuthentication extensions using ASPasskeyAssertionCredentialExtensionOutput and ASPasskeyRegistrationCredentialExtensionOutput as part of the ASPasskeyAssertionCredential and ASPasskeyRegistrationCredential objects you return to the system.

### Platform Single Sign-On

- Support stronger encryption and signing options by specifying supportedDeviceEncryptionAlgorithms, supportedDeviceSigningAlgorithms, and supportedUserSecureEnclaveKeySigningAlgorithms in the SSO extension. You can now use Hybrid Public Key Encryption (HPKE) algorithms defined in ASAuthorizationProviderExtensionEncryptionAlgorithm: `ecdhe_A256GCM`, `hpke_P256_SHA256_AES_GCM_256`, `hpke_P384_SHA384_AES_GCM_256`, and `hpke_Curve25519_SHA256_ChachaPoly`.

- If you use HPKE, receive notifications when the system rotates the encryption key by implementing keyWillRotate(for:newKey:loginManager:completion:) in your SSO extension. The system automatically rotates the encryption key about once per week. This lets you register the new key on the server.

- Rotate the keys you use for platform SSO by calling the ASAuthorizationProviderExtensionLoginManager methods beginKeyRotation(_:) and completeKeyRotation(_:).

## See Also

### Technology updates

Accelerate updates

Learn about important changes to Accelerate.

Accessibility updates

Learn about important changes to Accessibility.

ActivityKit updates

Learn about important changes in ActivityKit.

AdAttributionKit Updates

Learn about important changes to AdAttributionKit.

App Intents updates

Learn about important changes in App Intents.

AppKit updates

Learn about important changes to AppKit.

Apple Intelligence updates

Learn about important changes to Apple Intelligence.

Apple Pencil updates

Learn about important changes to Apple Pencil.

ARKit updates

Learn about important changes to ARKit.

Audio Toolbox updates

Learn about important changes to Audio Toolbox.

AVFAudio updates

Learn about important changes to AVFAudio.

AVFoundation updates

Learn about important changes to AVFoundation.

Bundle Resources updates

Learn about important changes to Bundle Resources.

ContactsUI updates

Learn about important changes to ContactsUI.

Core Location updates

Learn about important changes to Core Location.

