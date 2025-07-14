

- Bundle Resources
- Information Property List
-  NSAppleEventsUsageDescription 

Property List Key

# NSAppleEventsUsageDescription

A message that tells the user why the app is requesting the ability to send Apple events.

macOS 10.14+

## Details 

Name  
Privacy - AppleEvents Sending Usage Description

Type  

string

## Discussion

An app using Apple events to control another app might be able to gain access to sensitive user data. For example, the Mail app stores a lot of personal information in its local database that other apps can’t access directly. But because Mail can be automated with Apple events, other apps can use Mail to gain access to the data indirectly.

Important

This key is required if your app uses APIs that send Apple events.

## See Also

### Security

NSUpdateSecurityPolicy

A dictionary that identifies which apps or installer packages the operating system allows to write to the app’s bundle.

NSAppDataUsageDescription

A message that tells the user why the app needs to access files in other apps’ sandbox containers.

**Name:** Privacy - Other Application Data Usage Description

NSUserTrackingUsageDescription

A message that informs the user why an app is requesting permission to use data for tracking the user or the device.

**Name:** Privacy - Tracking Usage Description

NSSystemAdministrationUsageDescription

A message in macOS that tells the user why the app is requesting to manipulate the system configuration.

**Name:** Privacy - System Administration Usage Description

ITSAppUsesNonExemptEncryption

A Boolean value indicating whether the app uses encryption.

**Name:** App Uses Non-Exempt Encryption

ITSEncryptionExportComplianceCode

The export compliance code provided by App Store Connect for apps that require it.

**Name:** App Encryption Export Compliance Code

