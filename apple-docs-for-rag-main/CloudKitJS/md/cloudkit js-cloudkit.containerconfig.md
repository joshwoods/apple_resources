

- CloudKit JS
-  CloudKit.ContainerConfig 

Structure

# CloudKit.ContainerConfig

A configuration for a container.

CloudKit JS 1.0+

``` source
dictionary CloudKit.ContainerConfig {
 String containerIdentifier;
 String environment;
 String apnsEnvironment;
 Object apiTokenAuth;
 Object serverToServerKeyAuth;
};
```

## Overview

This table describes `apiTokenAuth` properties.

| Property | Description |
|----|----|
| `apiToken` | The API token generated and obtained using CloudKit Dashboard. To create an API token, read Accessing CloudKit Using an API Token in CloudKit Web Services Reference. |
| `persist` | Boolean value indicating whether the CloudKit session token persists. The default value is `false`. |
| `signInButton` | The sign-in button to display to the user. The properties are:  id: The DOM element ID. The default value is `apple-sign-in-button`.  theme: The button theme. The default value is `medium`.  If `null`, uses the default property values. |
| `signOutButton` | The sign-out button to display to the user. The properties are:  id: The DOM element ID. The default value is `apple-sign-out-button`.  theme: The button theme. The default value is `medium`.  If `null`, uses the default property values. |

This table describes `serverToServerKeyAuth` properties.

| Property | Description |
|----|----|
| `keyID` | A unique identifier for the key generated using CloudKit Dashboard. To create this key, read Accessing CloudKit Using a Server-to-Server Key in CloudKit Web Services Reference. |
| `privateKeyFile` | The path to the PEM encoded key file. |
| `privateKeyPassPhrase` | The pass phrase for the key. |

## Topics

### Instance Properties

apiTokenAuth

The API token and other authentication properties, described in the Discussion section. Either this key or the `serverToServerKeyAuth` key is required. If you include this key, don’t include the `serverToServerKeyAuth` key.

apnsEnvironment

The Apple Push Notification service (APNs) environment associated with this container. Possible values are CloudKit.DEVELOPMENT_ENVIRONMENT and CloudKit.PRODUCTION_ENVIRONMENT.

containerIdentifier

The string that identifies the app’s container. This key is required.

environment

The version of the app’s container. Possible values are CloudKit.DEVELOPMENT_ENVIRONMENT and CloudKit.PRODUCTION_ENVIRONMENT.

serverToServerKeyAuth

The server-to-server authentication key and related properties, described in the Discussion section. Either this key or the `apiTokenAuth` key is required. If you include this key, don’t include the `apiTokenAuth` key.

## See Also

### Structures

CloudKit.CloudKitConfig

Dictionary used to configure the CloudKit environment.

CloudKit.NameComponents

The parts of the user’s name.

CloudKit.NotificationInfo

Information about a notification.

CloudKit.Query

Search parameters to use when fetching records from the database.

CloudKit.Record

A record in the database.

CloudKit.RecordField

A field value of a record.

CloudKit.RecordInfo

Encapsulates the results of fetching information about a record.

CloudKit.RecordZone

Represents a record zone.

CloudKit.RecordZoneChanges

Represents the changes in a record zone.

CloudKit.RecordZoneChangesOptions

Options about fetching changes in a record zone.

CloudKit.Share

Represents a shared record.

CloudKit.ShareParticipant

Represents a user who accepted a shared record.

CloudKit.SharingUIResult

Represents the results of sharing a record with other users.

CloudKit.Subscription

A subscription, which is a persistent query on the server that tracks the creation, deletion, and modification of records.

CloudKit.UserIdentity

Information to identify a user.

