

- Xcode
- Capabilities
-  Configuring iCloud services 

Article

# Configuring iCloud services

Share user or app data among multiple instances of your app running on different devices.

## Overview

As an app developer, you can use one or more iCloud services to securely store your users’ data on the iCloud servers and make it available across all of their iCloud-enabled devices, thereby providing a seamless experience regardless of which device they use.

Xcode’s iCloud capability allows you to configure the following services:

- Key-value storage provides your app with 1 MB of iCloud storage that can contain up to 1024 key-value pairs, which is useful for syncing small amounts of data, such as the user’s preferences. For more information, see NSUbiquitousKeyValueStore.

- iCloud Documents allows your app to store data as files and sync those files across devices, which is relevant if your app is already using UIDocument or NSDocument. For more information, see Designing for Documents in iCloud.

- CloudKit allows your app to store structured objects and relationships in remote databases and provides full control over those databases’ schemas. Users can also choose to share their data with other iCloud users. You can use the CloudKit framework directly, or if your app uses Core Data to persist its data, leverage CloudKit to sync that data across devices. For more information, see Mirroring a Core Data store with CloudKit.

iCloud Documents and CloudKit both use *iCloud containers*, although their purpose differs depending on the service. For iCloud Documents, a container — alternatively known as a *ubiquity container* — serves as a local representation of the corresponding iCloud storage and is a specialized location on-disk where your app stores its files. For CloudKit, a container isolates your app’s databases on the iCloud servers and manages their access and operations. For more information, see CKContainer. You can also use containers to share files and data between multiple apps belonging to the same developer.

Before you can enable an iCloud service, follow the steps in the Add a capability section of Adding capabilities to your app to add the capability to your app’s target, and select the iCloud capability from Xcode’s Capabilities library. For watchOS apps with separate WatchKit extensions, add the capability to the WatchKit Extension target. To access a public iCloud database in your App Clip, add the capability to your App Clip target and be sure to read Choosing the right functionality for your App Clip for more information about using iCloud services in your App Clip.

After you add the iCloud capability, Xcode updates your target’s entitlements file to include the iCloud Container Identifiers Entitlement, which is an array that comprises the containers you select. If Xcode automatically manages your app’s signing, it also enables the iCloud capability for your app’s App ID in your developer account.

Note

If you later remove the iCloud capability in Xcode, you must manually update your App ID’s configuration in your developer account to disable iCloud.

### Enable one or more iCloud services

Prior to using an iCloud service to sync your users’ data across their devices, you must enable that service in Xcode to add the necessary entitlements to your app’s entitlements file. Use the checkbox next to the service’s name in the Services section of the iCloud capability to enable that service.

Depending on the services you enable, Xcode adds the following additional entitlements (if they’re not already present).

| Service           | Entitlement                                          |
|-------------------|------------------------------------------------------|
| Key-value storage | `com.apple.developer.ubiquity-kvstore-identifier`    |
| iCloud Documents  | `com.apple.developer.icloud-services`                |
|                   | `com.apple.developer.ubiquity-container-identifiers` |
| CloudKit          | `com.apple.developer.icloud-services`                |

For more information, see iCloud Key-Value Store Entitlement and iCloud Services Entitlement.

Note

Xcode automatically adds the Push Notifications capability to your target if you enable the CloudKit service because CloudKit uses push notifications to inform your app of server-side changes to your data. For more information, see Remote Records.

### Manage your app’s iCloud containers

After adding the iCloud capability, Xcode retrieves any existing iCloud containers from your developer account and displays them in the capability’s configuration section. Use the Refresh button below the list to re-fetch your account’s iCloud containers at any time.

Enable one or more iCloud containers in the list using their checkboxes. Conversely, uncheck a container’s checkbox to prevent your app from using it. Xcode associates the selected iCloud containers with your app’s App ID in your developer account and makes the following changes to your app’s entitlements file:

- For apps that enable iCloud Documents, or both iCloud Documents and CloudKit, Xcode updates the following entitlements to include the selected containers:

  - `com.apple.developer.icloud-container-identifiers`

  - `com.apple.developer.ubiquity-container-identifiers`

- Xcode updates just the `com.apple.developer.icloud-container-identifiers` entitlement for apps that enable only CloudKit.

Note

To avoid breaking existing versions of your app that depend on the container association, Xcode doesn’t automatically dissociate a deselected container from your App ID in your developer account.

To create a new iCloud container, perform the following steps:

1.  Click the Add button (+) below the iCloud containers list.

2.  Enter an iCloud container in the dialog that appears. You must begin the container’s name with `iCloud.` and use a unique string in reverse DNS notation.

3.  Click OK to save the new iCloud container.

Xcode automatically registers the iCloud container in your developer account, adds it to your app’s entitlements file, and selects it in the list of containers, indicating that your app is now able to use the new container.

After selecting the required containers, update your app to perform one or more of following:

- For document-based apps, call url(forUbiquityContainerIdentifier:) to determine the location of your app’s ubiquity container.

- For CloudKit apps, use init(identifier:) to initialize an instance of CKContainer that provides access to the container’s databases and executes operations against those databases.

- For Core Data apps that sync with CloudKit, use NSPersistentCloudKitContainerOptions to configure your Core Data stack to use your new container.

### Access the CloudKit console

If your app enables the CloudKit service, use the web-based CloudKit Console to manage all aspects of your app’s iCloud containers, including the schemas for their databases, operation logs, and performance telemetry. For more information, see Managing iCloud Containers with CloudKit Database App.

Follow these steps to access the CloudKit Console:

1.  Click the CloudKit Console button below the list of containers in the iCloud capability.

2.  In the browser window that opens, sign in to the CloudKit Console using the same Apple Account as your developer account.

Alternatively, you can access the console directly at icloud.developer.apple.com.

## See Also

### Data management

Configuring an associated domain

Create a two-way association between your app and your website to enable universal links, Handoff, App Clips, and shared web credentials.

Configuring app groups

Enable communication and data sharing between multiple installed apps created by the same developer.

