

- Device Management
-  DeclarativeManagementRequest 

Device Management Command

# DeclarativeManagementRequest

The declarative managmement request details.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object DeclarativeManagementRequest
```

## Properties

`Data`

`data`

A Base64-encoded JSON object using the SynchronizationTokens schema.

`Endpoint`

`string`

 (Required) 

The type of operation the declaration is requesting. This key must be one of these values:

- `tokens`: For fetching synchronization tokens from the server

- `declaration-items`: For fetching the declaration manifest from the server

- `status`: For sending a status report to the server

- `declaration/…/…`: For fetching a specific declaration from the server. Include the declaration type and identifier separated by forward slashes (`/)`.

`EnrollmentID`

`string`

 (Required) 

The per-enrollment identifier for the device.

`EnrollmentUserID`

`string`

 (Required) 

`MessageType`

`string`

 (Required) 

The message type, which must have a value of `DeclarativeManagement`.

Value: `DeclarativeManagement`

`UDID`

`string`

 (Required) 

`UserID`

`string`

`UserLongName`

`string`

 (Required) 

`UserShortName`

`string`

## Discussion

The `Data` field is optional, depending on the `Endpoint` value, as described below:

`tokens`  
The client uses the `tokens` endpoint to request the current synchronization tokens from the server. The `Data` field isn’t used. A successful response to this request is a `200 OK HTTP` status, with a response body that’s a JSON object conforming to the TokensResponse schema.

`declaration-items`  
The client uses the `declaration-items` endpoint to request the current declaration manifest from the server. The `Data` field isn’t used. A successful response to this request is a `200 OK HTTP` status, with a response body that’s a JSON object conforming to the DeclarationItemsResponse schema.

`declaration/…/…`  
The client uses the `declaration/…/…` endpoint to request a specific declaration from the server. The `Data` field isn’t used.

The endpoint value is a path with 3 segments separated by a / character. The first segment is always `declaration`. The second segment indicates the declaration type and is one of `activation`, `asset`, `configuration`, or `management`. The third segment is the `Identifier` of the declaration to fetch.

A successful response to this request is a `200 OK HTTP` status, with a response body that’s a JSON object representing the requested declaration. If the declaration isn’t present on the server, it must return a `404 Not Found HTTP` status response to the device. The device then considers that declaration to no longer exist on the server and removes any corresponding declaration present on the device.

`status`  
The client uses the `status` endpoint to send a status report to the server. The `Data` field must be present and set to a base64-encoded JSON object conforming to the StatusReport schema. A successful response to this request is a `200 OK HTTP` status, with an empty response body.

## Topics

### Declaration Endpoints

declaration/activation/{identifier}

The endpoint for fetching an activation declaration.

declaration/asset/{identifier}

The endpoint for fetching an asset declaration.

declaration/configuration/{identifier}

The endpoint for fetching a configuration declaration.

declaration/management/{identifier}

The endpoint for fetching a management declaration.

### Declaration Response

object DeclarationResponse

The details of a declaration, including its type and payload.

