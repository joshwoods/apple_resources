

- Technotes
-  TN3137: On Mac keychain APIs and implementations 

Article

# TN3137: On Mac keychain APIs and implementations

Learn how the keychain on macOS differs from other Apple platforms.

## Overview

All Apple platforms support the keychain. On iOS, tvOS, and watchOS the keychain story is very simple: There’s a single SecItem API with consistent behavior. This is not the case on macOS. The keychain on macOS has a long history, dating back to the previous millenium. This history, combined with a requirement to maintain compatibility with existing code, complicates the keychain’s design. If you don’t understand that design, you may find some of its behavior surprising.

macOS has three keychain APIs:

- Keychain. This originated on traditional Mac OS. Mac OS X supported it as a compatibility measure, and that support persists all the way through to the latest versions of macOS.

- SecKeychain. This was introduced with Mac OS X and was the standard macOS keychain API until the introduction of the SecItem API.

- SecItem. This was part of the original iOS SDK. macOS gained support for it in macOS 10.6.

Note

The Keychain API is declared in `` within the Core Services framework. The SecKeychain API is declared in ``, ``, and ``, all within the Security framework. The SecItem API is declared in ``, also within the Security framework.

macOS has two keychain implementations:

- File-based keychain

- Data protection keychain

The file-based keychain has its origins on traditional Mac OS. The data protection keychain originated on iOS and came to macOS with the advent of iCloud Keychain on macOS 10.9.

Important

iOS, tvOS, and watchOS only support the SecItem API with the data protection keychain implementation.

The Keychain and SecKeychain APIs always target the file-based keychain. The SecItem API can target either implementation. It defaults to targeting the file-based keychain. To target the data protection keychain, set the kSecUseDataProtectionKeychain attribute or the kSecAttrSynchronizable attribute to true.

The file-based keychain is on the road to deprecation. It’s not officially deprecated, but some of the APIs surrounding it are. For example, `SecKeychainCreate` was deprecated in the macOS 12 SDK. Moreover, new features, like iCloud Keychain, require the data protection keychain.

## Choosing the right keychain

Choosing a keychain API is easy: Use the SecItem API. If you have existing code that uses the older Keychain or SecKeychain APIs, consider updating it to use the SecItem API as part of your ongoing maintenance work.

Choosing a keychain implementation is more nuanced. Default to targeting the data protection keychain because:

- It behaves consistently across all Apple platforms.

- It benefits from new features, like iCloud Keychain.

- It has an access control model that’s both easier to understand and better aligned with current platform norms.

In some environments your only option is the data protection keychain, including:

- Mac Catalyst apps

- iOS Apps on Mac

In these environments you don’t need to supply the `kSecUseDataProtectionKeychain` attribute or the `kSecAttrSynchronizable` attribute to target the data protection keychain. It’s the default and only option. The system ignores the `kSecUseDataProtectionKeychain` attribute in these environments. If you have cross-platform keychain code, you may choose to simplify that code by setting `kSecUseDataProtectionKeychain` in all cases.

In other situations your only option is the file-based keychain:

- Programs that read existing items in a file-based keychain must target the file-based keychain. If you find yourself in this situation, consider migrating items to the data protection keychain as you update your app.

- Programs that run outside of a user context, like a `launchd` daemon, must target the file-based keychain. The data protection keychain is only available to programs running in a user context, like an app or an app extension.

## API differences

The SecItem API is well aligned with the data protection keychain. However, when you use it to target the file-based keychain it operates through a shim. That shim has limitations. Some of those limitations are inherent to the keychain implementation. For example, the access control model of the file-based keychain is completely different than that of the data protection keychain, and the shim can’t make up for that. However, some limitations are just bugs. To avoid such problems, target the data protection keychain. This is particularly important when you’re porting keychain code from iOS.

## Implementation differences

The data protection keychain is only available in a user login context. You can’t use it, for example, from a `launchd` daemon.

Each user gets exactly one data protection keychain. The system selects the correct keychain based on the context of the caller. That’s why the data protection keychain is only available in a user login context.

File-based keychains are stored, as the name suggests, in files. Every context has a keychain search list and a default keychain. In a user context the search list includes a per-user *login* keychain and a single *System* keychain, with the former being the default. In the system context the search list includes just the *System* keychain, which is also the default keychain.

When using the SecItem API to target the file-based keychain:

- SecItemAdd adds the item to the default keychain. Use kSecUseKeychain to override this.

- Queries, like those done using SecItemCopyMatching, consult all keychains in the search list. Use kSecMatchSearchList to override this.

Each keychain implementation uses its own access control model:

- The file-based keychain uses access control lists (`SecAccess`).

- The data protection keychain uses keychain access groups, supplemented by an optional access control object (SecAccessControl).

macOS builds the list of data protection keychain access groups available to your program from its code signing entitlements. For the details, see Sharing Access to Keychain Items Among a Collection of Apps. These entitlements must be authorized by a provisioning profile. Your program needs an app-like bundle structure in which to embed that profile. This is standard for app and app extensions but not for command-line tools. For information on how to wrap a command-line tool in a dummy app-like structure, see Signing a daemon with a restricted entitlement.

Important

This command-line tool will only work when run from a user context because, regardless of the packaging, the data protection keychain is only available in that context.

If you’re building library code, its data protection keychain access is determined by the entitlements of the host process’s main executable.

For more on provisioning profiles, see TN3125: Inside Code Signing: Provisioning Profiles.

The data protection keychain can hold all keychain item classes (Internet password, generic password, certificate, key). macOS 11 and later synchronize all classes; earlier versions synchronize only the password classes.

Some keychain features require the data protection keychain, including:

- iCloud Keychain. See the kSecAttrSynchronizable attribute.

- Protecting an item with biometrics (Touch ID and Face ID). See Restricting Keychain Item Accessibility.

- Protecting a key with the Secure Enclave. See Protecting keys with the Secure Enclave.

## User interface

The Keychain Access application supports both file-based keychains and the data protection keychain. The keychain list shows all the file-based keychains in the search list for the current user—typically this is just *login* and *System*—and the data protection keychain. It displays the latter as either *iCloud Keychain* or *Local Items*, depending on whether the user has enabled iCloud Keychain. To create, add, and remove a file-based keychain, choose the corresponding command on the File menu.

Keychain Access displays all keychain items in file-based keychains but only password items in the data protection keychain.

Keychain Access sometimes fails to reflect changes made to the keychain by other apps (r. 82556933). If you see unexpected results, quit and relaunch Keychain Access.

The keychain support in the `security` command-line tool is primarily focused on the file-based keychain.

## Revision History

- **2022-11-01** Republished as TN3137. Made significant editorial changes.

- **2021-12-10** First published as ”On Mac Keychains” on Apple Developer Forums.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

