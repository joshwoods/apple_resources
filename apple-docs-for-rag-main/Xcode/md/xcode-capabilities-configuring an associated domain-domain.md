

- Xcode
- Capabilities
-  Configuring an associated domain 

Article

# Configuring an associated domain

Create a two-way association between your app and your website to enable universal links, Handoff, App Clips, and shared web credentials.

## Overview

The system uses associated domains to initiate a secure association between your app and specific domains so they can share saved passwords, perform Handoff activities, and support universal links that allow users to open your app in a specific context and quickly complete their current task. To create such an association, you configure your app with the necessary entitlements by using Xcode to define associated domains, and then serve a special file from your web server that the system requires in order to verify those entitlements.

Before you can define associated domains and the services they provide, follow the steps in the Add a capability section of Adding capabilities to your app to add the capability to your app’s target, making sure you select the Associated Domains capability from Xcode’s Capabilities library. For watchOS apps with separate WatchKit extensions, add the capability to the WatchKit Extension target.

If not already present, Xcode updates your target’s entitlements file to include the Associated Domains Entitlement, which is an array that contains each associated domain you define. If you enable the “Automatically manage signing” option for your target, Xcode also updates your app’s App ID in your developer account and generates and downloads an updated provisioning profile.

Note

If you later remove the Associated Domains capability in Xcode, you must manually update your App ID’s configuration in your developer account to fully disable the feature.

### Define a service and its associated domain

When you want your app and one or more of your websites to interact using predefined services, define an associated domain by performing the following steps. Xcode automatically updates the `com.apple.developer.associated-domains` array in your target’s entitlements file to include those you define.

1.  Select your project in Xcode’s Project navigator.

2.  Select the app’s target in the Targets list.

3.  Click the Signing & Capabilities tab in the project editor.

4.  Find the Associated Domains capability.

5.  Click the Add button (+) to insert a service-domain placeholder.

6.  Double-click the inserted placeholder to edit it.

Update the placeholder to contain the service your app supports and its associated domain, which must be in the following format:

```
:
```

Only include the top-level domain and, where necessary, the subdomain; don’t include path and query components, or a trailing slash.

Tip

For services other than App Clips, prefix a domain with `*.` to include all of its subdomains.

The following table describes the services that associated domains support:

| Service | Description |
|----|----|
| `webcredentials` | If your domain supports shared web credentials, see Managing Shared Credentials for more information. |
| `authsrv` | If your domain needs to authenticate people, see Authenticating a User Through a Web Service for more information. |
| `applinks` | If your domain supports universal links, see Supporting universal links in your app for more information. |
| `activitycontinuation` | If your domain supports Handoff, see Web Browser-to-Native App Handoff for more information. |
| `appclips` | If your domain supports App Clips, see Associating your App Clip with your website for more information. |

### Provide an Apple App Site Association file

When the user installs your app that contains associated domains, the system fetches the corresponding *Apple App Site Association* (AASA) file from an Apple-managed content delivery network (CDN) and uses its JSON contents to verify those associated domains. If the CDN doesn’t store a copy of that file, or has an outdated version, it automatically connects to your server and retrieves the latest version.

After you define your app’s associated domains in Xcode, you must create this file and serve it using HTTPS from your website’s `.well-known` directory. For more information, see Add the associated domain file to your website.

### Enable alternate mode for unreachable servers

If you use a private web server while developing your app that’s unreachable from the public internet, enable *alternate mode* — an option you specify that allows the system to bypass Apple’s CDN and fetch the AASA file directly from your web server.

Follow these steps to enable alternate mode on a specific associated domain:

1.  Select your project in Xcode’s Project navigator.

2.  Select the app’s target in the Targets list.

3.  Click the Signing & Capabilities tab in the project editor.

4.  Find the Associated Domains capability.

5.  Double-click the associated domain in the Domains list to edit it.

6.  Append the string `?mode=` to the associated domain. Replace `` with one of the modes shown in the list below.

7.  Press Return to save the updated associated domain.

The following table describes the alternate modes that associated domains support:

| Mode | Description |
|----|----|
| `developer` | The domain is accessible from devices with Developer Mode enabled. You must sign the app with a development profile and users must opt-in on their device by enabling the Associated Domains Development option in Settings \> Developer. |
| `managed` | The domain is accessible from devices using a mobile device management (MDM) profile and that have authorization from the MDM administrator. |
| `developer+managed` | The domain is accessible only from devices that are in both `developer` and `managed` modes. |

Important

Only use alternate mode during development; you must remove the query string from the associated domains before you submit your app to the App Store.

## See Also

### Data management

Configuring app groups

Enable communication and data sharing between multiple installed apps created by the same developer.

Configuring iCloud services

Share user or app data among multiple instances of your app running on different devices.

