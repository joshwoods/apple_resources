

- MarketplaceKit
-  MarketplaceKitError 

Enumeration

# MarketplaceKitError

Errors that can occur in the marketplace workflow.

iOS 17.4+iPadOS 17.4+

``` source
enum MarketplaceKitError
```

## Overview

The AppLibrary variety of functions `requestAppInstallation(...)` can throw an error of this type.

## Topics

### Enumeration Cases

case appNotInstalled

The requested operation cannot be completed because the app isn’t installed

case cancelled

The app isn’t eligible to be installed

case featureUnavailable

The requested feature is unavailable

case installationOfMarketplaceDenied

Installations of marketplaces are denied on this device.

case installationRestricted

Installations are restricted on this device.

case insufficientStorageSpace(Measurement&lt;UnitInformationStorage>)

The requested install requires more storage space than the device has available.

case invalidAlternativeDistributionPackageSignature

The signature of the Alternative Distribution Package wasn’t available or was invalid

case invalidAlternativeDistributionPackageURL

Invalid URL for an Alternative Distribution Package

case invalidLicense

No valid license provided

case invalidManifest

The manifest is invalid, or cannot be read

case invalidURL

An invalid URL was provided

case minimumPlatformVersionNotSatisfied(String)

The requested install requires a minimum platform version that is greater than this device.

case mismatchedInstallType

The provided install type doesn’t match the install that would occur

case missingCapabilities([String])

The requested install requires capabilities not available on this device.

case missingInstallVerificationToken

The required install verification token is missing

case networkError

A network error occurred during the request

case noSupportedVariant

The requested install has no supported variant for this device.

case oauthTokenError

An error fetching an OAuth Token

case ratingRestricted

The requested install has a rating that exceeds this device’s restrictions.

case unknown

Failure due to an unknown error.

case unsupportedPlatform

The requested install does not run on this device’s platform.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var description: String

A textual representation of this instance.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Default Implementations

Error Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Decodable
- Encodable
- Error
- Sendable

