

- Bundle Resources
- Information Property List
-  NSUserTrackingUsageDescription 

Property List Key

# NSUserTrackingUsageDescription

A message that informs the user why an app is requesting permission to use data for tracking the user or the device.

iOS 14.0+iPadOS 14.0+tvOS 14.0+visionOS 1.0+

## Details 

Name  
Privacy - Tracking Usage Description

Type  

string

## Discussion

If your app calls the App Tracking Transparency API, you must provide custom text, known as a *usage-description string*, which displays as a system-permission alert request. The usage-description string tells the user why the app is requesting permission to use data for tracking the user or the device. The user has the option to grant or deny the authorization request. If you don’t include a usage-description string, your app may crash when a user first launches it.

Make sure your app requests permission to track sometime before tracking occurs. This could be at first launch or when using certain features in your app. For example, when signing on with a third-party SSO. For more information on asking permission to track, see User privacy and data use.

Set the NSUserTrackingUsageDescription key in the Information Property List (`Info.plist`):

1.  Select your project’s `Info.plist` file in Xcode Project navigator.

2.  Modify the file using the Xcode Property List Editor: Privacy - Tracking Usage Description.

- Use sentence-style capitalization and appropriate ending punctuation. Keep the text short and specific. You don’t need to include your app name because the system already identifies your app.

- If the title is a sentence fragment, don’t add ending punctuation.

See Apple’s Human Interface Guidelines for example usage descriptions.

## See Also

### Security

NSUpdateSecurityPolicy

A dictionary that identifies which apps or installer packages the operating system allows to write to the app’s bundle.

NSAppDataUsageDescription

A message that tells the user why the app needs to access files in other apps’ sandbox containers.

**Name:** Privacy - Other Application Data Usage Description

NSAppleEventsUsageDescription

A message that tells the user why the app is requesting the ability to send Apple events.

**Name:** Privacy - AppleEvents Sending Usage Description

NSSystemAdministrationUsageDescription

A message in macOS that tells the user why the app is requesting to manipulate the system configuration.

**Name:** Privacy - System Administration Usage Description

ITSAppUsesNonExemptEncryption

A Boolean value indicating whether the app uses encryption.

**Name:** App Uses Non-Exempt Encryption

ITSEncryptionExportComplianceCode

The export compliance code provided by App Store Connect for apps that require it.

**Name:** App Encryption Export Compliance Code

