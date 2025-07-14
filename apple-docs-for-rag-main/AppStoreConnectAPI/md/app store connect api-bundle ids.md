

- App Store Connect API
-  Bundle IDs 

API Collection

# Bundle IDs

Manage the bundle IDs that uniquely identify your apps.

## Overview

The `bundleIds` resource represents the app’s unique identifier that you can register, modify, and delete. You need a bundle ID before you can assign capabilities with the Bundle ID Capabilities resource or create a provisioning profile with the Profiles resource.

## Topics

### Registering Bundle IDs

Register a New Bundle ID

Register a new bundle ID for app development.

### Modifying and Removing Bundle IDs

Modify a Bundle ID

Update a specific bundle ID’s name.

Delete a Bundle ID

### Getting Bundle ID Information

List Bundle IDs

Find and list bundle IDs that are registered to your team.

Read Bundle ID Information

Get information about a specific bundle ID.

### Getting Related Data

Read the App Information of a Bundle ID

List All Profiles for a Bundle ID

Get a list of all profiles for a specific bundle ID.

List All Capabilities for a Bundle ID

Get a list of all capabilities for a specific bundle ID.

### Objects and Types

object BundleId

The data structure that represents a Bundle IDs resource.

type BundleIdPlatform

Strings that represent the operating system intended for the bundle.

object BundleIdCreateRequest

The request body you use to create a Bundle ID.

object BundleIdUpdateRequest

The request body you use to update a Bundle ID.

object BundleIdResponse

A response that contains a single Bundle IDs resource.

object BundleIdWithoutIncludesResponse

object BundleIdsResponse

A response that contains a list of Bundle ID resources.

## See Also

### Provisioning

Bundle ID Capabilities

Manage the app capabilities for a bundle ID.

Certificates

Create, download, and revoke signing certificates for app development and distribution.

Devices

Register devices for development and testing.

Profiles

Create, delete, and download provisioning profiles that enable app installations for development and distribution.

Merchant ID

Manage your merchant ID for Apple Pay.

