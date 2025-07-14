

- CloudKit JS
-  CloudKit.CloudKitConfig 

Structure

# CloudKit.CloudKitConfig

Dictionary used to configure the CloudKit environment.

CloudKit JS 1.0+

``` source
dictionary CloudKit.CloudKitConfig {
 CloudKit.ContainerConfig[] containers;
 Object services;
};
```

## Overview

The table describes the `services` properties.

| Property | Description |
|----|----|
| `logger` | An object with methods `info`, `log`, `warn`, and `error`. You can set this to `window.console`. |
| `fetch` | A function compatible with `window.fetch`. |
| `Promise` | An object used for deferred and asynchronous computations. To learn more, go to Mozilla Developer Network: Promise. |
| `authTokenStore` | An object with these two methods:  `putToken(containerIdentifier:String, authToken:String) -> void;`  `getToken(containerIdentifier:String) -> String;` |

## Topics

### Instance Properties

containers

An array of dictionaries used to configure each container of type CloudKit.ContainerConfig.

services

Encapsulates information about services, described in the Discussion section.

## See Also

### Structures

CloudKit.ContainerConfig

A configuration for a container.

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

