

- Updates
-  File Provider updates 

Article

# File Provider updates

Learn about important changes to File Provider.

## Overview

Browse notable changes in File Provider.

## June 2024

- Offer people the ability to sync their Desktop and Documents folders with your File Provider app. Check whether a person opts in to sync these folders using replicatedKnownFolders. Sync the folders using claimKnownFolders(_:localizedReason:completionHandler:), or stop syncing using releaseKnownFolders(_:localizedReason:completionHandler:) if the person opts out. Provide the system with information about which folders you support syncing through supportedKnownFolders, and share the locations of the folders by adopting NSFileProviderKnownFolderSupporting.

- Cache files on external disks. Confirm whether a volume is eligible for storing a domain using checkDomainsCanBeStoredOnVolume(at:), and create a domain on that volume using the new init(displayName:userInfo:volumeURL:) initializer. Store data about the current sync state using stateDirectoryURL(), and determine whether to connect to a domain created on another device using shouldConnectExternalDomain(completionHandler:).

- Install the File Provider logging profile to log helpful information for debugging and troubleshooting. Download the `.mobileconfig` file at Profiles and Logs.

## March 2024

- Improve error handling with new underlying error codes for NSFileProviderError.Code.providerNotFound. NSFileProviderError.Code.providerDomainTemporarilyUnavailable indicates that the system is unable to service requests for this domain temporarily, and you can try again later. NSFileProviderError.Code.providerDomainNotFound indicates that there isn’t a registered domain for the corresponding identifier. NSFileProviderError.Code.applicationExtensionNotFound indicates that there isn’t an app extension within the app bundle.

## See Also

### Technology updates

Accelerate updates

Learn about important changes to Accelerate.

Accessibility updates

Learn about important changes to Accessibility.

ActivityKit updates

Learn about important changes in ActivityKit.

AdAttributionKit Updates

Learn about important changes to AdAttributionKit.

App Intents updates

Learn about important changes in App Intents.

AppKit updates

Learn about important changes to AppKit.

Apple Intelligence updates

Learn about important changes to Apple Intelligence.

Apple Pencil updates

Learn about important changes to Apple Pencil.

ARKit updates

Learn about important changes to ARKit.

Audio Toolbox updates

Learn about important changes to Audio Toolbox.

AuthenticationServices updates

Learn about important changes to AuthenticationServices.

AVFAudio updates

Learn about important changes to AVFAudio.

AVFoundation updates

Learn about important changes to AVFoundation.

Bundle Resources updates

Learn about important changes to Bundle Resources.

ContactsUI updates

Learn about important changes to ContactsUI.

