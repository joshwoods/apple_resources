

- Bundle Resources
- Information Property List
-  ITSAppUsesNonExemptEncryption 

Property List Key

# ITSAppUsesNonExemptEncryption

A Boolean value indicating whether the app uses encryption.

macOS 10.0+

## Details 

Name  
App Uses Non-Exempt Encryption

Type  

boolean

## Discussion

Set the value for this key to `NO` in your app’s Information Property List file to indicate that your app—including any third-party libraries you link against—either uses no encryption, or only uses encryption that’s exempt from export compliance requirements, as described in Determine your export compliance requirements. Set the value to `YES` to indicate that your app uses non-exempt encryption.

If you set the value to `YES`, you typically also provide a value for the ITSEncryptionExportComplianceCode key. You set that key’s value using a code Apple provides after successfully reviewing your export compliance documentation.

If you don’t have the ITSAppUsesNonExemptEncryption key in your app’s `Info.plist` file, App Store Connect walks you through an export compliance questionnaire every time you upload a new version of your app. Including the key streamlines the app submission process.

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

ITSEncryptionExportComplianceCode

The export compliance code provided by App Store Connect for apps that require it.

**Name:** App Encryption Export Compliance Code

