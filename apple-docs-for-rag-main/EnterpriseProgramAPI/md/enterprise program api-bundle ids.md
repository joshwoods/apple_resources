

- Enterprise Program API
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

Modify a PassTypeId

Update a specific bundle ID’s name.

Delete a BundleId

Delete a bundle ID that is used for app development.

### Getting Bundle ID Information

List Bundle Ids

Find and list bundle IDs that are registered to your team.

Read BundleId Information

Get information about a specific bundle ID.

### Getting Related Data

List All Profiles for a BundleId

Get a list of all profiles for a specific bundle ID.

List All Bundle Id Capabilities for a BundleId

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

A response that contains a single Bundle IDs resource without includes.

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

Pass Type Ids

Create, download, and revoke pass type ids for app development and distribution.

Profiles

Create, delete, and download provisioning profiles for development and distribution.

