

- Technotes
-  TN3125: Inside Code Signing: Provisioning Profiles 

Article

# TN3125: Inside Code Signing: Provisioning Profiles

Learn how provisioning profiles enable third-party code to run on Apple platforms.

## Overview

Code signing is a foundational technology on all Apple platforms. Many documents that discuss code signing focus on solving a specific problem. The *Inside Code Signing* technote series is different: It peeks behind the code signing curtain, to give you a better understanding of how this technology works. Read these technotes to make better code signing choices up front, to understand why Apple’s code signing tools work the way they do, to inform your investigation of any code signing issues you encounter, and because learning stuff is fun!

The other technotes in the *Inside Code Signing* series are:

- TN3126: Inside Code Signing: Hashes

- TN3127: Inside Code Signing: Requirements

- TN3161: Inside Code Signing: Certificates

Important

The *Inside Code Signing* technotes discuss code signing details that aren’t considered API. The structure of a code signature has changed numerous times in the past and may well change again in the future. Don’t encode this information in your product. When signing code, use Xcode (all platforms) or the `codesign` tool (macOS only). To get information or validate a code signature, use the `codesign` tool or the Code Signing Services API. Apple updates these facilities to accommodate any changes to the code signature structure as they roll out.

## Provisioning profile fundamentals

Apple platforms, except macOS, won’t run arbitrary third-party code. All execution of third-party code must be authorized by Apple. This authorization comes in the form of a provisioning profile, which ties together five criteria:

- Who is allowed to sign code?

- What apps are they allowed to sign?

- Where can those apps run?

- When can those apps run?

- How can those apps be entitled?

Note

In this document the term *app* refers to a main executable packaged in a bundle structure. This encompasses apps, app extensions, App Clips, system extensions, and XPC Services.

You create provisioning profiles using the Apple Developer website, either directly using the website or indirectly using Xcode or the App Store Connect API.

When the Apple Developer website creates a profile for you, it cryptographically signs it. When you run an app on a device, the device checks this signature to determine if the profile is valid and, if so, checks that the app meets the criteria in the profile.

Note

Unlike Apple’s other platforms, macOS doesn’t require a provisioning profile to run third-party code. However, provisioning profiles are still relevant on macOS, as explained in Entitlements on macOS.

There is one interesting edge case with provisioning profiles: When you submit your app to the App Store, the App Store re-signs the app as part of the distribution process. Before doing that, it checks that the app is signed and provisioned correctly. That check means that each individual device doesn’t need to perform further security checks, so the final app doesn’t have a provisioning profile. However, this third-party code was still authorized by a profile, albeit during the App Store distribution process.

## Unpack a profile

A provisioning profile is a property list wrapped within a Cryptographic Message Syntax (CMS) signature. To view the original property list, remove the CMS wrapper using the `security` tool:

```
```

For more details on CMS, see RFC 5652.

Important

The exact format of provisioning profiles isn’t documented and could change at any time. Use the techniques shown here for understanding and debugging purposes. Avoid building a product based on these details; if you do build such a product, be prepared to update it as the Apple development story evolves.

To illustrate this point, the traditional property list view of a profile is no longer the source of truth on modern systems. Rather, each profile contains a `DER-Encoded-Profile` property which holds a binary form of the profile that’s the new source of truth. For more on this switch, see The Future is DER.

Still, the property list is easier to read and so the bulk of this technote focuses on that.

For more information about the tools used in these examples, read their man pages. If you’re unfamiliar with that process, see Reading UNIX Manual Pages.

## The who

Every profile has a `DeveloperCertificates` property holding the certificates of each developer who can sign code covered by the profile. For example:

```
```

To extract a specific certificate, add its index to the key path:

```
```

To learn more about code-signing certificates, read TN3161: Inside Code Signing: Certificates.

## The what

Most profiles apply to a single App ID, encoded in the `Entitlements` \> `application-identifier` property:

```
```

Note

On macOS the standard App ID entitlement is `com.apple.application-identifier`. A Mac Catalyst app uses both `com.apple.application-identifier` and `application-identifier`.

This property holds an App ID, composed of an App ID prefix and a bundle ID. In this example `SKMME9E2Y8` is the App ID prefix and `com.example.apple-samplecode.ProfileExplainer` is the bundle ID.

A profile might refer to a wildcard App ID:

```
```

This profile applies to any app whose App ID starts with `SKMME9E2Y8.com.example.apple-samplecode.`

## The where

Most profiles apply to a specific list of devices. This is encoded in the `ProvisionedDevices` property:

```
```

App Store distribution profiles have no `ProvisionedDevices` property because you can’t run an App Store distribution signed app locally.

Developer ID and In-House (Enterprise) distribution profiles have the `ProvisionsAllDevices` property, indicating that they apply to all devices. For more details about Developer ID provisioning profiles on the Mac, see Entitlements on macOS.

## The when

Every profile has an `ExpirationDate` property which limits how long the profile remains valid. For example:

```
```

This validity period varies by profile type, but it’s typically not more than a year. The exception here is Developer ID profiles, which have an expiration date far in the future.

## The how

Every profile has an `Entitlements` property which authorizes the app to use specific entitlements. For example:

```
```

The entitlements in the profile act as an allowlist. This isn’t the same as the entitlements claimed by the app. To actually claim an entitlement, include the entitlement in the app’s code signature.

Every entitlement claimed by the app must be in the profile’s allowlist but the reverse isn’t true. It’s fine for the allowlist to include entitlements that the app doesn’t claim.

Note

A macOS app can claim certain entitlements without them being authorized by a provisioning profile. For more on this, see Entitlements on macOS.

Some entitlements in the allowlist use wildcard syntax. In the above example, `SKMME9E2Y8.*` means that the app can claim any keychain access group with the `SKMME9E2Y8.` prefix. Wildcards don’t make sense in the app’s code signature.

To dump the entitlements claimed by the app, use `codesign` with the `--entitlements` argument:

```
```

Note

By default `--entitlements` dumps a human-readable representation of the DER-encoded entitlements. The above example uses `--xml` to force it to output XML. It runs the output through `plutil` to pretty print that XML. To learn more about DER in provisioning profiles, see The Future is DER.

Every entitlement claimed by this app is authorized by its profile, and thus iOS allows the app to run. Note that the `keychain-access-groups` value, `SKMME9E2Y8.com.example.apple-samplecode.ProfileExplainer`, starts with `SKMME9E2Y8.` and thus is allowed by the wildcard.

## Entitlements on macOS

A macOS app can claim certain entitlements without them being authorized by a provisioning profile. These *unrestricted entitlements* include:

- `com.apple.security.get-task-allow`

- `com.apple.security.application-groups`

- Those used to enable and configure the App Sandbox

- Those used to configure the Hardened Runtime

Note

On other Apple platforms the equivalent to `com.apple.security.get-task-allow` is `get-task-allow` and, as with all entitlements on those platforms, must be authorized by a profile. Also, App Groups work differently on macOS and other platforms. For details, see App Groups Entitlement.

In contrast, *restricted entitlements* must be authorized by a provisioning profile. This is an important security feature on macOS. For example, the fact that the `keychain-access-groups` entitlement must be authorized by a profile means that other developers can’t impersonate your app in order to steal its keychain items.

A Mac app that uses no restricted entitlements doesn’t need a provisioning profile. This is true even if the app is distributed on the App Store. The only exception to this rule is TestFlight, which always requires a profile.

macOS supports provisioning profiles for both App Store and Developer ID distribution. Some entitlements are not supported by Developer ID profiles. For the details, see Supported capabilities (macOS) in Developer Account Help. For general information about Developer ID signing, see Signing Mac Software with Developer ID

## Profile location

In the early days of iOS development it was common to install a provisioning profile on the device as a whole (in the Settings app). That’s still possible, but current best practice is to embed the profile within the app itself:

- macOS expects to find the profile at `MyApp.app/Contents/embedded.provisionprofile`.

- Other Apple platforms expect to find the profile at `MyApp.app/embedded.mobileprovision`.

Note that macOS also uses a different file name extension for provisioning profiles.

Apps that you download from the App Store don’t contain an embedded provisioning profile because the App Store checks that the app is signed and provisioned correctly as part of its distribution process.

Some macOS products, like daemons and command-line tools, ship as a standalone executable. A standalone executable can’t claim a restricted entitlement because there’s no place to embed the provisioning profile that authorizes that claim. If your standalone executable needs to do this, wrap it in an app-like structure. For an example of this, see Signing a Daemon with a Restricted Entitlement.

## The future is DER

Modern systems no longer treat the profile’s property list as the source of truth. Rather, they use the binary form of the profile stored in the profile’s `DER-Encoded-Profile` property:

```
```

This form of the profile is encoded as DER, a binary encoding of ASN.1 that’s common in cryptographic file formats. To extract it, first extract the property to a file:

```
```

This is a whole new copy of the profile, so undo the CMS wrapper again:

```
```

Finally, dump the DER-encoded payload itself:

```
```

This output contains mostly the same information as the property list, just encoded in DER form.

The one exception is the `DeveloperCertificates` property. This doesn’t contain a full copy of each certificate, but rather a SHA-256 checksum of the certificate. Assuming the certificate extracted from the property list earlier as `cert0.cer`, run `shasum` to confirm that checksum:

```
```

This DER-encoded profile is required starting with iOS 15, iPadOS 15, tvOS 15, and watchOS 8. For more on that change, see Using the Latest Code Signature Format.

## Revision History

- **2024-02-06** Added a link to TN3126: Inside Code Signing: Hashes. Made other minor editorial changes.

- **2022-05-24** Made minor editorial changes.

- **2022-05-03** Republished as TN3125. Added The Future is DER section. Updated the examples to use `plutil`. Also made significant editorial changes.

- **2021-07-26** First published as ”What exactly is a provisioning profile?” on Apple Developer Forums.

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

