

- Device Management
-  AppManaged 

Object

# AppManaged

The declaration to configure a managed app.

iOS 17.2+iPadOS 17.2+visionOS 2.4+Device Assignment ServicesVPP License Management

``` source
object AppManaged
```

## Properties

`AppConfig`

AppManagedAppConfigDictionaryObject

A dictionary of app config data and credentials.

`AppStoreID`

`string`

The App Store ID of the managed app.

`Attributes`

AppManagedAttributesObject

A dictionary of values to associate with the app.

`BundleID`

`string`

The bundle ID of the managed app.

`ExtensionConfigs`

AppManagedExtensionConfigsObject

A dictionary of extension config data and credentials.

`IncludeInBackup`

`boolean`

If `true`, backups contain the app and its data.

Default: `true`

`InstallBehavior`

AppManagedInstallBehaviorObject

A dictionary that describes how and when to install the app.

`LegacyAppConfigAssetReference`

`string`

The identifier of an asset declaration containing a reference to the app config data. This app config data is applied and made available to the app using the traditional MDMv1 behavior. The corresponding asset must be of type `com.apple.asset.data`. The referenced data must be a property list file, and the asset’s “ContentType” value should be set to match the data type.

`ManifestURL`

`string`

The URL of the manifest for the managed app.

## Discussion

Provide a value for one and only one of the `AppStoreID`, `BundleID`, or `ManifestURL` keys.

Note

This documentation contains preliminary information about an API or technology in development. This information is subject to change. Learn more about using Apple’s beta software.

## Topics

### Objects

object AppManagedAppConfigDictionaryObject

A dictionary of app config data and credentials.

object AppManagedAttributesObject

A dictionary of values associated with an app.

object AppManagedCredentialConfigObject

A dictionary of values associated with a credential config.

object AppManagedExtensionConfigsObject

A dictionary of values associated with an extension config.

object AppManagedInstallBehaviorObject

A dictionary that describes how and when to install an app.

## See Also

### Configurations

object AccountCalDAV

The declaration to configure a Calendar account.

object AccountCardDAV

The declaration to configure an address book account.

object AccountExchange

The declaration to configure an Exchange account.

object AccountGoogle

The declaration to configure a Google account.

object AccountLDAP

The declaration to configure a Lightweight Directory Access Protocol (LDAP) account.

object AccountMail

The declaration to configure a Mail account.

object AccountSubscribedCalendar

The declaration to configure a Calendar subscription.

object DiskManagementSettings

The declaration to configure disk management settings on the device.

object LegacyInteractiveProfile

The declaration to configure an interactive, legacy profile.

object LegacyProfile

The declaration to configure a legacy profile.

object ManagementStatusSubscriptions

The declaration to configure status subscriptions.

object ManagementTest

The declaration to test the MDM system.

object MathSettings

The declaration to configure the math and calculator apps.

object PasscodeSettings

The declaration to configure passcode policy settings.

object SafariExtensionSettings

The declaration to configure Safari Extensions.

