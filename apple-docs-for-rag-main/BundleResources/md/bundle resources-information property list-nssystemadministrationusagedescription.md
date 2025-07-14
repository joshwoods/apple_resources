

- Bundle Resources
- Information Property List
-  NSSystemAdministrationUsageDescription 

Property List Key

# NSSystemAdministrationUsageDescription

A message in macOS that tells the user why the app is requesting to manipulate the system configuration.

macOS 10.14+

## Details 

Name  
Privacy - System Administration Usage Description

Type  

string

## Discussion

Use this key if your app uses certain APIs that manipulate system configuration, like ODRecordSetValue(_:_:_:_:).

Important

This key is required if your app uses APIs that manipulate the system configuration.

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

NSAppleEventsUsageDescription

A message that tells the user why the app is requesting the ability to send Apple events.

**Name:** Privacy - AppleEvents Sending Usage Description

ITSAppUsesNonExemptEncryption

A Boolean value indicating whether the app uses encryption.

**Name:** App Uses Non-Exempt Encryption

ITSEncryptionExportComplianceCode

The export compliance code provided by App Store Connect for apps that require it.

**Name:** App Encryption Export Compliance Code

