

- CloudKit JS
-  CloudKit.NotificationInfo 

Structure

# CloudKit.NotificationInfo

Information about a notification.

CloudKit JS 1.0+

``` source
dictionary CloudKit.NotificationInfo {
 String alertBody;
 String alertLocalizationKey;
 String[] alertLocalizationArgs;
 String alertActionLocalizationKey;
 String alertLaunchImage;
 String soundName;
 Boolean shouldBadge;
 Boolean shouldSendContentAvailable;
 String[] additionalFields;
 String category;
};
```

## Overview

The `CloudKit.NotificationInfo` dictionary is the same as the dictionary described in Notification Info Dictionary in CloudKit Web Services Reference.

## Topics

### Instance Properties

additionalFields

Fields the server sends along with this notification.

alertActionLocalizationKey

A key to get a localized right button title that appears in the alert dialog.

alertBody

The text of the alert message.

alertLaunchImage

The filename of an image file in the app bundle used as a launch image.

alertLocalizationArgs

Array of strings to appear as variables if `alertLocalizationKey` is a format specifier.

alertLocalizationKey

A key to a localized alert-message.

category

The name of the action group corresponding to this notification.

shouldBadge

A Boolean value indicating whether a badge should be displayed. If `true`, a badge is displayed; otherwise, it is not. The default value is `false`.

shouldSendContentAvailable

A Boolean value indicating whether new content is available. If `true`, new content is available; otherwise, it is not. The default value is `false`.

soundName

The name of a sound file in the app bundle to play as an alert.

## See Also

### Structures

CloudKit.CloudKitConfig

Dictionary used to configure the CloudKit environment.

CloudKit.ContainerConfig

A configuration for a container.

CloudKit.NameComponents

The parts of the user’s name.

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

