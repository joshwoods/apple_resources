

- MarketplaceKit
-  Ingesting an alternative distribution package 

Article

# Ingesting an alternative distribution package

Process an available app version from App Store Connect and store it for download from your server.

## Overview

When an app passes Notarization, App Store Connect makes it available for storage on the back end of your web server. The app format that App Store Connect provides is an *alternative distribution package*, which contains everything a device needs to install the available app. App Store Connect sends newly available apps that an alternative marketplace app distributes to your web server automatically through your notifications webhook; see Processing alternative app marketplace notifications. For your apps that install from your website, you need to download your alternative distribution package from App Store Connect manually.

In either case, to prepare the package for installation on devices, process, or *ingest*, the package to a specific format, and serve its contents from specific relative locations that the operating system expects.

## Receive new package version notification

If the developer of an app that your marketplace distributes enables notifications in App Store Connect, your webhook receives the `AlternativeDistributionPackageVersionAvailable` notification when a new version of that app is available. For information about enabling notifications, see Manage distribution on an alternative app marketplace.

When your webhoook receives `AlternativeDistributionPackageVersionAvailable`, check the notification’s `attributes` object for the app ID and version. For example:

```
```

In the POST body, the alternative distribution package version ID refers to the specific available alternative distribution package. To begin retrieving actual app data from App Store Connect, pass `alternativeDistributionPackageVersionId` as the `id` path parameter to the `alternativeDistributionPackageVersions/{id}` endpoint, as follows:

```
GET https://api.appstoreconnect.apple.com/v1/alternativeDistributionPackageVersions/6B29FC40-CA47-1067-B31D-00DD010662DA
```

For more information about the `alternativeDistributionPackageVersions/{id}` endpoint, see Read information for an alternative distribution package version.

Example response:

```
```

In the response, navigate to the `data.attributes.url`, which downloads `alternative-distribution-package.zip`. Inside the `zip` file is a manifest and a signature:

| File | Description |
|----|----|
| `manifest.json` | Instructions you use to assemble the alternative distribution package. |
| `signature` | A signature that the device’s operating system uses to verify the package contents. |

Tip

Save the `alternativeDistributionPackageId` in case you want to query App Store Connect for all alternative distribution package versions outside of a normal `AlternativeDistributionPackageVersionAvailable` notification. For more information, see Read alternative distribution package information.

For more information on alternative distribution package workflows, see Alternative Distribution Packages.

## Process the manifest file

The manifest file contains links to assets that you download to compose a complete alternative distribution package. The individual assets represent unique variations and portions of an app, as required to install it on the variety of Apple devices that the app supports.

An example manifest follows:

```
```

When the operating system installs an app on a device, it accesses your server at different subfolders off the base URL you provide in the download link depending on the needs of the requesting device. When your endpoint processes the alternative distribution package, you ingest and organize the contents that the manifest references according to two categories:

*Variants*  
Complete app bundles that vary slightly to support different device types.

*Deltas*  
Partial app bundles, that consist of just the bits required to update from one version of an app to another.

## Download app variants

The variants reside at the top of the manifest. The first variant in the example has a `publicId` of `219750db-80c2-4c75-aecc-fa67835f384d`. To download the variant, provide the `publicId` as the `id` path parameter of the `alternativeDistributionPackageVariants` endpoint, as follows:

```
GET https://api.appstoreconnect.apple.com/alternativeDistributionPackageVariants/219750db-80c2-4c75-aecc-fa67835f384d
```

For more information about the `alternativeDistributionPackageVariants` endpoint, see Read information for an alternative distribution package variants.

Example response:

```
```

In the response, navigate to the `data.attributes.url`, which downloads `pre-thinned11331259484252926706.thinned.signed.dpkg.ipa`, which is an installable app for the particular class of supported devices that Apple assigns this variant. Although an app that resides on App Store Connect might contain binaries for multiple platforms, the alternative distribution package sent to the marketplace only contains variants for the platforms that MarketplaceKit supports. For example, a specific alternative distribution package that a marketplace receives contains only iPhone or iPad variants; it doesn’t contain watch variants.

The `alternativeDistributionKeyBlob` (*key blob*) has a unique value for each variant. The App License Delivery SDK requires the key blob during licensing requests. Store the key blob so your licensing service can use it to decrypt the license request payload coming from a device as required to generate an app license for the variant.

## Download app deltas

If someone already has a prior version of the app installed, the system selects a delta to install rather than a variant. The deltas reside at the bottom of the manifest. The first delta in the example has a `publicId` of `ffbc52b6-f76b-4d51-9eff-5388bc6b7572`. To download the first delta, provide the `publicId` as the `id` path parameter of the `alternativeDistributionPackageDeltas` endpoint, as follows:

```
GET https://api.appstoreconnect.apple.com/alternativeDistributionPackageDeltas/ffbc52b6-f76b-4d51-9eff-5388bc6b7572
```

For more information about the `alternativeDistributionPackageDeltas` endpoint, see Read information for alternative distribution package deltas.

Example response:

```
```

Important

When App Store Connect sends a new app version notification, it sends an app distribution package that includes the variants first, followed by another for deltas, if any are available for the app. Deltas arrive an unspecified amount of time after the app’s variants. You don’t need to wait for deltas to arrive before serving the new app to devices. Rather, App Store Connect sends variants first to expedite the app’s availability for customers.

## Store the app data at an expected path

Assemble all of the downloaded alternative distribution package assets into a folder structure, as follows:

```
delta/
manifest.json
signature
variant/
```

You can serve the base URL of this file structure from any URL scheme you choose. When the device’s operating system attempts to download the app, it accesses the contents of this folder according to the `alternativeDistributionPackage` parameter that you provide to either:

- MarketplaceKitURIScheme URLs, when serving your app marketplace

- The InstallMetadata initializer init(account:appleItemID:alternativeDistributionPackage:isUpdate:), when serving apps that reside on your marketplace

Store the variants and deltas according to their `assetPath` in the manifest. For example, the following `assetPath` tells you how to name a specific variant and where to store it off the base URL:

```
"assetPath": "variant/219750db-80c2-4c75-aecc-fa67835f384d.ipa",
```

When the device’s operating system attempts to download an app, it first reads the manifest to discover the contents of the alternative distribution package, then the operating system reads the signature to validate the variant or delta it chooses to install.

## Validate the assembled app data

You can use the `dist_package_tool` utility on macOS 14.4 and later to verify the integrity of the alternative distribution packages you assemble. After downloading and assembling a complete alternative distribution package, you can validate it with the command:

```
```

This utility verifies the signature in the manifest and that the folders contain the correct assets that the manifest references.

The `-v` option provides verbose output. The following example represents the output of a valid alternative distribution package:

```
Validating package: file:///Users//476476a1-6246-4782-98f1-9ca3819827ad/
Package has a valid signature.
All resources are present and valid.
```

If the alternative distribution package is incomplete, the output can identify problems. For example:

```
Package contained added files.
    Added file: .DS_Store
Package contained missing files.
    Missing file: variant/7e11a118-ab90-4a52-9ca1-31362f5d108e.ipa
```

The tool’s return value indicates success or failure, so you can branch conditional logic using it in a script.

## See Also

### Web services

Processing alternative app marketplace notifications

Manage the addition and removal of apps available on your alternative marketplace.

Installing your app from your website

Manage the installation of an app that you develop and distribute through your website.

Installing apps from an alternative marketplace

Manage the installation of apps that developers distribute from your marketplace app.

Supplying an install verification token

Support the installation of alternative distribution apps by creating signed JSON web tokens.

