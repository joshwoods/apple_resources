

- Device Management
- App and Book Management
-  Upgrading to the new App and Book Management API 

Article

# Upgrading to the new App and Book Management API

Manage devices and content across your organization using the new API version.

## Overview

New features and improved asynchronous processing in App and Book Management API 2 enable MDMs to manage apps and books in a faster and more scalable way than ever before. To take advantage of these new features, MDMs need to change the way in which they manage apps and books.

For more information, see Managing Apps and Books Through Web Services. For an overview of what’s new in version 2, watch the WWDC21 presentation Improve MDM assignment of Apps and Books.

### Understand endpoint changes

The following table shows the differences between the API 1 and API 2 endpoints. For more information about specific API protocols and usage, see App and Book Management.

| Version 1 | HTTP method | Version 2 | HTTP method |
|----|----|----|----|
| `editVPPUserSrv` | POST | `users/update` | POST |
| `getAssignments` | POST | `assignments` | GET |
| `getVPPAssetsSrv` | POST | `assets` | GET |
| `getVPPLicensesSrv` | POST |  |  |
| `getVPPUsersSrv`  `getVPPUserSrv` | POST | `users` | GET |
| `manageVPPLicensesByAdamIdSrv` | POST | `assets/associate`  `assets/disassociate` | POST |
| `registerVPPUserSrv` | POST | `users/create` | POST |
| `retireVPPUserSrv` | POST | `users/retire` | POST |
| `VPPClientConfigSrv` | POST | `client/config`  `client/config` | POST  GET |
| `VPPServiceConfigSrv` | POST | `service/config` | GET |
|  |  | `status` | GET |
|  |  | `assets/revoke` | POST |

### Track assignments

Assignment tracking in version 2 is very similar to that in version 1; however, version 2 no longer supports the use of license IDs. To simplify the management process, version 2 deprecates the `getVPPLicensesSrv` endpoint. This means that MDMs can no longer use Apple-assigned IDs to identify their license assignments.

To properly identify an assignment through Get Assignments, version 2 uses the combination of `adamId` and `clientUserId` for user-based assignments, or `adamId` and `serialNumber` for device-based assignments. An MDM can also use the `adamId` alone to retrieve all assignments for that `adamId`.

### Use pagination

In version 1, results batch through a `batchToken` if the total number of records exceeds the limit results. With batches, the initial request occurs with no `batchToken`. The response includes `batchToken` with the first batch of records if the number of records exceeds a server-controlled limit. To get the next batch of records, the MDM needs to include the batch token in the subsequent requests. Using Paginated Endpoints is version 2’s solution to work with larger result sets more efficiently.

In the new API, when the number of records in a response exceeds a server-controlled limit, the server paginates the response. Endpoints that support pagination, such as Get Assets and Get Users, can accept a page index query parameter. Using the page index, you can access a response page directly; you don’t need to access pages sequentially. Additionally, to reduce the time it takes to retrieve the full set, an MDM can make paginated requests in parallel.

### Batch requests

In version 1, all asset management calls occur synchronously. It’s the MDM’s responsibility to batch large requests and send them in parallel to Apple. This results in sending many small simultaneous requests to Apple, which sometimes leads to resource contention and failed requests. With version 2, MDMs can send a single, much larger request and rely on Apple to batch the request and process it asynchronously, enforcing parallelism on the server. This results in processing optimization, which fulfills large requests more quickly and more reliably.

To take advantage of batching, MDMs can discontinue the use of small, parallel management requests and, instead, group similar Associate Assets and Disassociate Assets tasks into a single, larger request. An MDM can perform thousands of assignments or unassignments in a single request. The Service Config response specifies the maximum number of `adamIds`, `clientUserIds,` and `serialNumbers` the version 2 management requests accept.

### Subscribe to notifications

Subscribing to Notifications in version 2 provides a huge improvement to the tracking of the latest events for MDMs. MDMs no longer require fetching on assignment endpoints to confirm the results of management requests. MDMs can configure a notification host and send notifications to the MDMs upon the completion of asset and user-management requests.

In addition to receiving notifications for MDM-initiated events, an MDM may also receive a notification for user-initiated events, such as asset purchases and transfers.

For information about subscribing to different notification types, see ClientConfigRequest.

### Set MDM information

In version 2, when creating a ClientConfigRequest, the MDM can include MdmInfo in the request. The server returns this information on all subsequent responses to identify which MDM is managing the location. It’s important to interrogate the `MdmInfo` content API responses to ensure no other MDM is attempting to manage the data in this location.

Within `MdmInfo`, the MDMs have the opportunity to include `metadata`, a free-form field to store additional information for the organization. Note: In version 2, `metadata` replaces `clientContext` from version 1. It’s advisable to include informative plain text descriptors, particularly in the `name` field, to help identify the MDM in the case of any discrepancies. Once an MDM uses version 2, the `clientContext` in version 1 for that location is automatically updated to display ‘token being used in v2’.

### Perform occasional syncs

Notifications remove the necessity for MDMs to continually sync with Apple for asset and user counts, which occurs frequently in version 1. However, it’s a best practice for MDMs to occasionally sync their data using Get Assets, Get Users, or Get Assignments to avoid missing notifications, especially when an MDM doesn’t initiate a request.

### Sanitize MDM information

To maintain MDM hygiene, update the `mdmInfo` field using the Client Config endpoint to reflect any changes. Prior to releasing a location, remove any assets assigned to a location through transferring. If an MDM is failing to receive notifications, it’s preferable to sanitize the `notificationUrl` field and reset it to a reachable url.

## See Also

### Essentials

Managing Apps and Books Through Web Services

Associate app and book purchases with users or devices.

Apps and Books for Organizations

Get details about apps and books to show to your users.

Managing Assets

Retrieve key information to effectively manage assets across an organization’s users and devices.

Managing Users

Retrieve key information to effectively manage users across an organization.

Using Paginated Endpoints

Manage paginated endpoints to efficiently work with large record sets.

Subscribing to Notifications

Listen to notifications to keep track of the latest events for an organization.

Handling Error Responses

Investigate service request errors and troubleshoot solutions.

