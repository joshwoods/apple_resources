

- Enterprise Program API
-  Pass Type Ids 

API Collection

# Pass Type Ids

Create, download, and revoke pass type ids for app development and distribution.

## Overview

The `passTypeId` resource represents a pass type certificates unique identifier that you can register, modify, and delete. You need a pass type ID before you can create a pass type certificate with the Certificates resource.

## Topics

### Managing Pass Type Ids

Create a PassTypeId

Create a new identifier for use with a pass type ID certificate using a certificate signing request.

List Pass Type Ids

Find and list pass type IDs that are registered to your team.

Read PassTypeId Information

Get information about a specific pass type ID.

List All Certificates for a PassTypeId

List all certificates for a specific pass type ID.

Modify a PassTypeId

Update a specific pass type ID’s name.

Delete a PassTypeId

Delete a pass type ID that is used for app development.

### Getting Pass Type Id Infomation and Data

Read the Pass Type Id Information of a Certificate

### Object and Data Types

object PassTypeId

The data structure that represents a pass type ID.

object PassTypeIdCreateRequest

The request body you use to create a pass type ID.

object PassTypeIdResponse

A response that contains a pass type ID resource.

object PassTypeIdsResponse

A response that contains a list of pass type ID resources.

object PassTypeIdUpdateRequest

The request body you use to update a pass type ID name.

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

Profiles

Create, delete, and download provisioning profiles for development and distribution.

