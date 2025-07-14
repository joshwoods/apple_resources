

- Bundle Resources
- Information Property List
-  NSAppDataUsageDescription 

Property List Key

# NSAppDataUsageDescription

A message that tells the user why the app needs to access files in other apps’ sandbox containers.

macOS 14.0+

## Details 

Name  
Privacy - Other Application Data Usage Description

Type  

string

## Discussion

When your app tries to open a file that’s in another app’s sandbox container, the system requests permission from the person using the app and presents this message. If your app doesn’t have a value for the `NSAppDataUsageDescription` key in its information property list, the system presents a default message.

The system uses this message any time your app tries to access files in another app’s container, and your app can’t provide different messages for attempts to access containers from different apps.

## See Also

### Security

NSUpdateSecurityPolicy

A dictionary that identifies which apps or installer packages the operating system allows to write to the app’s bundle.

NSUserTrackingUsageDescription

A message that informs the user why an app is requesting permission to use data for tracking the user or the device.

**Name:** Privacy - Tracking Usage Description

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

