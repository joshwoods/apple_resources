

- App Store Connect API
-  Profiles 

API Collection

# Profiles

Create, delete, and download provisioning profiles that enable app installations for development and distribution.

## Overview

The `profiles` resource represents the provisioning profiles that allow you to install apps on your iOS devices or Mac. You can create and delete provisioning profiles, and download them to sign your code.

Provisioning profiles include signing certificates, device identifiers, and a bundle ID.

## Topics

### Creating and Deleting Provisioning Profiles

Create a Profile

Create a new provisioning profile.

Delete a Profile

Delete a provisioning profile that is used for app development or distribution.

### Getting Provisioning Profile Information

List and Download Profiles

Find and list provisioning profiles and download their data.

Read and Download Profile Information

Get information for a specific provisioning profile and download its data.

### Getting Related Data

Read the Bundle ID in a Profile

Get the bundle ID information for a specific provisioning profile.

List All Certificates in a Profile

Get a list of all certificates and their data for a specific provisioning profile.

List All Devices in a Profile

Get a list of all devices for a specific provisioning profile.

### Objects

object Profile

The data structure that represents a Profiles resource.

object ProfileCreateRequest

The request body you use to create a Profile.

object ProfileResponse

A response that contains a single Profiles resource.

object ProfilesResponse

A response that contains a list of Profiles resources.

object ProfilesWithoutIncludesResponse

## See Also

### Provisioning

Bundle IDs

Manage the bundle IDs that uniquely identify your apps.

Bundle ID Capabilities

Manage the app capabilities for a bundle ID.

Certificates

Create, download, and revoke signing certificates for app development and distribution.

Devices

Register devices for development and testing.

Merchant ID

Manage your merchant ID for Apple Pay.

