

- UIKit
- Protecting the User’s Privacy
-  Requesting access to protected resources 

Article

# Requesting access to protected resources

Provide a purpose string that explains to a person why you need access to protected resources on their device.

## Overview

Modern devices collect and store a wealth of sensitive information about people who use them. Many apps rely on this kind of data, and the device hardware that generates it, to do useful work. For example, a navigation app needs a person’s GPS coordinates to locate the person on a map. But not all apps need access to all data. The same navigation app doesn’t need access to a person’s health history, camera interface, or Bluetooth peripherals.

Ensure your app accesses only what it needs to do its job. To support this principle, Apple’s operating systems restrict access to protected data and resources by default. Apps can request access on a case-by-case basis, providing an explanation for why they need access. The person who uses the app decides whether to grant or deny the request.

Tip

In addition to asking people for permission to access a resource, in some cases, you also need to separately declare your intent to do so by adding an entitlement to your app, as described in Entitlements.

### Provide a purpose string

The first time your app attempts to access a protected resource, the system prompts the person using the app for permission. In the following example, an iOS app called FoodDeliveryApp, which provides a food delivery service, generates a prompt requesting access to the person’s location:

If the person grants permission, the system remembers the person’s choice and doesn’t prompt again. If the person denies permission, the access attempt that initiates the prompt, and any further attempts, fail in a resource-specific way. For the particular case of access to location data, the person can choose to allow access for one session only by tapping Allow Once.

The system automatically generates the prompt’s title, which includes the name of your app. You supply a message called a *purpose string* or a *usage description* — in this case, “Your location allows you to view restaurants in delivery range of your address.” — to indicate the reason that your app needs the access. Accurately and concisely explaining to the person why your app needs access to sensitive data, typically in one complete sentence, lets the person make an informed decision and improves the chances that they grant access.

You provide a purpose string by setting a string value for a resource-specific key that you add to your app’s Information Property List file. The message in the image above, for example, is a string associated with the NSLocationWhenInUseUsageDescription key. Modify your `Info.plist` file using the property list editor in Xcode.

Always provide a valid purpose string in the `Info.plist` file if your app uses a protected resource. If you don’t, attempts to access the resource fail, and might even cause your app to crash.

If your app supports multiple locales, in addition to providing a purpose string in the `Info.plist` file, localize it, and place the localized string in the `InfoPlist.strings` files for each locale you want to support.

### Adhere to the requirements for purpose strings

To give people useful, concise information about why you’re requesting access to protected resources, make sure each purpose string you provide is valid by checking the following:

- The purpose string isn’t blank and doesn’t consist solely of whitespace characters.

- The purpose string is shorter than 4,000 bytes. Typical purpose strings are one complete sentence, but you can provide additional information to help a person make the right decision about sharing personal information.

- The purpose string has the proper type that the corresponding key requires, typically a string.

- The purpose string provides a description that’s accurate, meaningful, and specific about why the app needs to access the protected resource.

Adhere to these requirements for every purpose string in the `Info.plist` file and locale-specific `InfoPlist.strings` files.

App Review checks for the use of protected resources, and rejects apps that contain code accessing those resources without a purpose string. For example, an app accessing location might receive the following information from App Review about the requirement that an NSLocationWhenInUseUsageDescription key be present:

```
```

To resolve this issue, provide a purpose string that explains why the app needs access to this sensitive information, or remove the code that’s accessing the resource.

Note

If you’re using external libraries or SDKs, they may reference APIs that require a purpose string. Although your app might not use these APIs, a purpose string is still necessary for App Review. You can contact the developer of the library or SDK to request information about which protected resources the developer uses and their purpose, or request that the developer release a version of their code that doesn’t contain the APIs. You’re responsible for all access of protected resources, including external SDK and library access.

### Check for authorization

Many system frameworks that provide access to protected resources have dedicated APIs for checking and requesting authorization to use those resources. This model allows you to adjust your app’s behavior depending on the current access it has. For example, if a person denies your app permission to do something, you can remove related elements from your user interface.

Because a person can change authorization at any time using Settings, always check the authorization status of a feature before accessing it. In cases without a dedicated API, prepare your app to gracefully handle access failures.

### Reset authorization access

When your app attempts to access a protected resource after its first attempt, the system remembers the person’s permission choice and doesn’t prompt again. To prompt the person again, you need to reset access to these resources on your device or system.

To reset permission access to a protected resource in iOS apps, tap Settings \> General \> Transfer or Reset iPhone \> Reset \> Reset Location & Privacy on your device.

Important

Using Reset Location & Privacy resets location and privacy settings for all services on your device.

To reset permissions for a particular service in macOS apps, run the `tccutil reset ` command in Terminal. For example, to reset all permissions for AppleEvents, type:

```
$ tccutil reset AppleEvents
```

This command resets authorization access for all apps using the protected resource. You can similarly specify Camera, Calendar, Reminders, or other services to reset them individually.

## See Also

### Supporting Privacy

Encrypting Your App’s Files

Protect the user’s data in iOS by encrypting it on disk.

