

- UIKit
-  UICloudSharingController 

Class

# UICloudSharingController

A view controller that presents standard screens for adding and removing people from a CloudKit share record.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UICloudSharingController
```

## Overview

CloudKit Sharing provides real-time collaboration between one or more people using your app. A user takes certain steps to make collaboration possible, from inviting people to participate in the collaboration to setting restrictions on what participants can do. To provide these steps to a user, you must make changes to your app. With UICloudSharingController, the changes require minimum effort.

The UICloudSharingController view controller class provides screens, presented within your app, for managing the people, permissions, and access rights associated with a CKShare record. The controller, along with a few lines of your own code, facilitates the setup and management of online sharing between users, making it possible for a user to:

- Invite people to view or collaborate on a shared record

- Set the access rights determining who can access the shared record (only people invited or anyone with the share link)

- Set general or individual permissions (read-only or read/write)

- Remove access from one or more participants

- Stop participating (if the user is a participant)

- Stop sharing with all participants (if the user is the owner of the shared record)

The controller provides these different actions to the user based on the user’s role. If the user is the individual sharing the record (where the record is an instance of CKRecord representing the data to share), then the user is called the *owner*. A user who has access to the shared record and isn’t the owner is known as a *participant*. There’s no need for you to specify the user’s role. The controller determines the role automatically.

### Inviting participants to a new share

The user who owns the data, represented as a CKRecord, can invite others to view or collaborate on changes to the data. To invite participants, the owner sends the share link to the other people. To provide this capability in your app, create an instance of UICloudSharingController using the init(preparationHandler:) initializer method. You use this initializer method only when the owner isn’t already sharing the record.

After creating the controller, you present it. The controller displays the Invitation screen. Using this screen, the owner can add participants and set restrictions on the shared record. Once done, the owner sends the share link to the participants.

However, before the owner can send the share link, CloudKit must generate the link. This link generation happens when saving a new CKShare record, but when do you save it? You save the share record in the `preparationHandler:`.

After the owner’s selections are complete, the controller invokes the preparation handler provided in the initializer call. In the handler, you create a new CKShare instance, initializing it with the CKRecord instance that represents the data to share. (This record is called the “root record.”) Next, you save the share and root records using CKModifyRecordsOperation. Finally, you return the shared record to the controller or return an error if the save failed. See the following code for an example of this in action.

- Swift
- Objective-C

```
func presentCloudSharingController(_ sender: Any) {  guard
    let barButtonItem = sender as? UIBarButtonItem,
    let rootRecord = self.recordToShare else {
    return
  }

  let cloudSharingController = UICloudSharingController { [weak self] (controller, completion: @escaping (CKShare?, CKContainer?, Error?) -> Void) in
    guard let `self` = self else {
      return
    }
    self.share(rootRecord: rootRecord, completion: completion)
  }

  if let popover = cloudSharingController.popoverPresentationController {
    popover.barButtonItem = barButtonItem
  }
  self.present(cloudSharingController, animated: true) {}
}

func share(rootRecord: CKRecord, completion: @escaping (CKShare?, CKContainer?, Error?) -> Void) {
  let shareRecord = CKShare(rootRecord: rootRecord)
  let recordsToSave = [rootRecord, shareRecord]
  let container = CKContainer.default()
  let privateDatabase = container.privateCloudDatabase
  let operation = CKModifyRecordsOperation(recordsToSave: recordsToSave, recordIDsToDelete: []) 
  operation.perRecordCompletionBlock = { (record, error) in
    if let error = error {
      print("CloudKit error: \(error.localizedDescription)")
    }
  }

  operation.modifyRecordsCompletionBlock = { (savedRecords, deletedRecordIDs, error) in
    if let error = error {
      completion(nil, nil, error)
    } else {
      completion(shareRecord, container, nil)
    }
  }

  privateDatabase.add(operation)
}
```

```
- (void)presentCloudSharingController:(id)sender
{
  CKRecord *rootRecord = [self recordToShare];
  if (rootRecord == nil || [sender isKindOfClass:[UIBarButtonItem class]] == NO) {
    return;
  }
  UICloudSharingController *cloudSharingController = [[UICloudSharingController alloc] initWithPreparationHandler:^(UICloudSharingController * _Nonnull controller, void (^ _Nonnull preparationCompletionHandler)(CKShare * _Nullable, CKContainer * _Nullable, NSError * _Nullable)) {

    [self shareRootRecord:rootRecord completion:preparationCompletionHandler];

  }];

  UIPopoverPresentationController *popover = [cloudSharingController popoverPresentationController];
  if (popover) {
    [popover setBarButtonItem:sender];
  }
  [self presentViewController:cloudSharingController animated:YES completion:nil];
}
- (void)shareRootRecord:(CKRecord *)rootRecord completion:(void (^)(CKShare * _Nullable share, CKContainer * _Nullable container, NSError * _Nullable error))completion
{
  CKShare *shareRecord = [[CKShare alloc] initWithRootRecord:rootRecord];
  NSArray *recordsToSave = @[rootRecord, shareRecord];
  CKContainer *container = [CKContainer defaultContainer];
  CKDatabase *privateDatabase = [container privateCloudDatabase];

  CKModifyRecordsOperation *operation = [[CKModifyRecordsOperation alloc] initWithRecordsToSave:recordsToSave recordIDsToDelete:@[]];
  [operation setPerRecordCompletionBlock:^(CKRecord * _Nullable record, NSError * _Nullable error) {
    if (error) {
      NSLog(@"%@", [error localizedDescription]);
    }
  }];
  [operation setModifyRecordsCompletionBlock:^(NSArray * _Nullable savedRecords, NSArray * _Nullable deletedRecordIDs, NSError * _Nullable error) {
    if (error) {
      NSLog(@"%@", [error localizedDescription]);
    }
    completion(shareRecord, container, error);
  }];

  [privateDatabase addOperation:operation];
}
```

### Adding and removing participants from an existing share

To allow the owner of an existing share to manage the participants, create the UICloudSharingController instance using the init(share:container:) initializer method.

After you create the controller, present it to show the People screen. From this screen, the owner can:

- Add and remove participants

- Change the share’s access options from private to public, or public to private

- Change the share’s permissions from read-only to read/write, or vice versa

- Stop sharing with all participants

Note

If all participants have left the share, the controller presents the Invitation screen, not the People screen, when init(share:container:) is used to create the controller instance.

### Viewing participants and leaving a share

To allow a participant to view the list of participants and remove themselves from a share, create the UICloudSharingController instance using the init(share:container:) initializer method.

After you create the controller, present it to show the People screen. From this screen, the participant can:

- View the list of participants

- Copy the share link to send to others (if the owner has made the share publicly available)

- Leave the share

### Presenting the controller

UICloudSharingController is designed for use in a popover. Therefore, you should always set the popoverPresentationController source information before presenting the Cloud sharing controller. Doing this ensures that the UICloudSharingController instance is displayed properly across all device types.

Important

Presenting the Cloud sharing controller in an iPad app without setting the popover presentation controller causes a run-time error.

The following code shows an example of setting the popoverPresentationController before presenting a Cloud sharing controller.

- Swift
- Objective-C

```
func presentCloudSharingController(_ sender: Any) {  guard
    let barButtonItem = sender as? UIBarButtonItem,
    let rootRecord = self.recordToShare else {
    return
  }

  let cloudSharingController = UICloudSharingController { (controller, completion: @escaping (CKShare?, CKContainer?, Error?) -> Void) in    
    // Save the share and root records.
    // Call completion(share, container, error) handler.
  }

  if let popover = cloudSharingController.popoverPresentationController {
    popover.barButtonItem = barButtonItem
  }
  self.present(cloudSharingController, animated: true) {}
}
```

```
- (void)presentCloudSharingController:(id)sender
{
  if ([self recordToShare] == nil || [sender isKindOfClass:[UIBarButtonItem class]] == NO) {
    return;
  }

  UICloudSharingController *cloudSharingController = [[UICloudSharingController alloc] initWithPreparationHandler:^(UICloudSharingController * _Nonnull controller, void (^ _Nonnull preparationCompletionHandler)(CKShare * _Nullable, CKContainer * _Nullable, NSError * _Nullable)) {
    // Save the share and root records
    // Call preparationCompletionHandler(share, container, error);
  }];

  UIPopoverPresentationController *popover = [cloudSharingController popoverPresentationController];
  if (popover) {
    [popover setBarButtonItem:sender];
  }

  [self presentViewController:cloudSharingController animated:YES completion:nil];
}
```

### Configuring the controller

By default, the UICloudSharingController user interface displays a generic thumbnail image and title to the user. You can, however, change these to app-specific representations of the shared record. You accomplish this by setting the controller’s delegate property to an object that conforms to the UICloudSharingControllerDelegate protocol, making sure to implement the itemThumbnailData(for:) and itemTitle(for:) delegate methods.

You can also show or hide the permission and access options presented to the user by setting the availablePermissions property on the UICloudSharingController instance.

## Topics

### Creating the cloud sharing controller

init(preparationHandler: (UICloudSharingController, (CKShare?, CKContainer?, (any Error)?) -> Void) -> Void)

Initializes the CloudKit sharing controller with a preparation handler intending to save a new share record.

Deprecated

init(share: CKShare, container: CKContainer)

Initializes the CloudKit sharing view controller with a CloudKit share record and container to manage participants and restrictions.

### Customizing the cloud sharing controller behavior

var delegate: (any UICloudSharingControllerDelegate)?

A reference to an object that conforms to the CloudKit sharing controller delegate protocol.

protocol UICloudSharingControllerDelegate

The protocol you implement to provide additional information to, and receive notifications from, the CloudKit sharing controller.

### Configuring the permissions

var availablePermissions: UICloudSharingController.PermissionOptions

A combination of permission and access options made available to the user when viewing screens presented by the CloudKit sharing controller.

struct PermissionOptions

A set of options that determine the permission options available to the user when viewing the Cloud sharing controller screens.

### Getting the share

var share: CKShare?

A reference to the CloudKit share record used by the CloudKit sharing controller.

### Getting an activity item source

func activityItemSource() -> any UIActivityItemSource

The activity item object that can be used by an activity view controller.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

