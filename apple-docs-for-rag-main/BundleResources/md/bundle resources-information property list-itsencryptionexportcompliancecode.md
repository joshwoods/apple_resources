

- Bundle Resources
- Information Property List
-  ITSEncryptionExportComplianceCode 

Property List Key

# ITSEncryptionExportComplianceCode

The export compliance code provided by App Store Connect for apps that require it.

macOS 10.0+

## Details 

Name  
App Encryption Export Compliance Code

Type  

string

## Discussion

Include this key in your app’s Information Property List file if you set the ITSAppUsesNonExemptEncryption key’s value to `YES`. Set the value for this key to the code that Apple sends you after successfully reviewing export compliance documentation that you provide through App Store Connect.

For additional information, see Complying with Encryption Export Regulations.

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

NSSystemAdministrationUsageDescription

A message in macOS that tells the user why the app is requesting to manipulate the system configuration.

**Name:** Privacy - System Administration Usage Description

ITSAppUsesNonExemptEncryption

A Boolean value indicating whether the app uses encryption.

**Name:** App Uses Non-Exempt Encryption

