

- Xcode
- Capabilities
-  Configuring app groups 

Article

# Configuring app groups

Enable communication and data sharing between multiple installed apps created by the same developer.

## Overview

An *app group* allows multiple apps developed by the same team to access one or more shared containers. It also enables additional interprocess communication (IPC) between those apps using Mach IPC, POSIX semaphores and shared memory, and UNIX domain sockets, among other IPC mechanisms. In macOS, app groups can facilitate communication between sandboxed apps, and between sandboxed and nonsandboxed apps. Apps can belong to one or more app groups. You can also use an app group to share data between an app extension or App Clip and its host app.

Before creating an app group, follow the steps in Add a capability to add the App Groups Entitlement to your app’s target.

### Create app groups

After adding the app groups capability to your app, Xcode retrieves any existing groups from your developer account and displays them in the capability’s section. Use the Refresh button below the app groups list to re-fetch your account’s groups at any time. Each developer account can register a maximum of 1,000 app groups.

To register an app group, see Register an app group. You need to register app groups for iOS, iPadOS, tvOS, visionOS, and watchOS apps.

Enable one or more groups in the list by selecting their checkboxes to add your app as a member of those groups. Conversely, uncheck a group’s checkbox to revoke your app’s membership.

To create an app group for your app, perform the following:

1.  Click the Add button (+) below the App Groups list.

2.  Enter a container ID in the dialog that appears. A container ID must begin with `group.` and then a custom string.

3.  Click OK to save the new app group.

Xcode automatically selects the new app group in the App Groups list; this selection indicates that your app is now a member of that app group.

Note

You can also create macOS app groups using the naming convention `.`. By using this naming scheme, macOS checks that the code signature of processes that try to access the app group container contains the same `Developer-Team-ID` as app group container ID.

### Access an app group’s shared container

When your app becomes a member of an app group, there are a number of APIs you can use to read and write data to that group’s shared container, such as:

- Sharing preferences and other limited data by using the init(suiteName:) method to access the app group’s shared user defaults database.

- Retrieving the physical location of the app group’s shared container by calling the containerURL(forSecurityApplicationGroupIdentifier:) method, which you can later use to read and write data.

- Set the sharedContainerIdentifier property on the configuration of a background URL session to download files directly into the app group’s shared container.

## See Also

### Data management

Configuring an associated domain

Create a two-way association between your app and your website to enable universal links, Handoff, App Clips, and shared web credentials.

Configuring iCloud services

Share user or app data among multiple instances of your app running on different devices.

