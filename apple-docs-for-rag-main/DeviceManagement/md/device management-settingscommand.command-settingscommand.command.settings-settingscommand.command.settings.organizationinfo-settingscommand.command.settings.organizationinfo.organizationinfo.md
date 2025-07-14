

- Device Management
- SettingsCommand
- 
  - SettingsCommand
- SettingsCommand.Command
- SettingsCommand.Command.Settings
- SettingsCommand.Command.Settings.OrganizationInfo
-  SettingsCommand.Command.Settings.OrganizationInfo.OrganizationInfo 

Device Management Command

# SettingsCommand.Command.Settings.OrganizationInfo.OrganizationInfo

A dictionary that contains information about the organization operating the MDM server.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object SettingsCommand.Command.Settings.OrganizationInfo.OrganizationInfo
```

## Properties

`OrganizationAddress`

`string`

The organization’s address. Use the LF character (`&#10`) to insert line breaks.

`OrganizationEmail`

`string`

The orgnization’s support email address.

`OrganizationMagic`

`string`

A unique identifier for the various services a single organization manages.

`OrganizationName`

`string`

 (Required) 

A string that describes the organization operating the MDM server for display to the user during certain operations, such as purchasing or installing apps.

`OrganizationPhone`

`string`

The organization’s phone number.

`OrganizationShortName`

`string`

A shorter version of `OrganizationName`, preferably a single word or abbreviation, suitable for display to the user in places where a very short name is necessary.

