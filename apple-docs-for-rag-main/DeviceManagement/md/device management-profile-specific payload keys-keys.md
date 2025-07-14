

- Device Management
-  Profile-Specific Payload Keys 

API Collection

# Profile-Specific Payload Keys

Use the appropriate payload for your configuration needs.

## Overview

In addition to the standard payload keys (described in Define a Profile) each payload can contain keys specific to a payload type. These payload specific keys are described in detail, below.

For profiles that use paths, consider them to be case sensitive.

## Topics

### Top Level

object TopLevel

The top-level payload properties you use to configure all profiles.

object CommonPayloadKeys

The payload properties that are common across all profiles.

### Accounts

object Accounts

The payload you use to configure guest accounts.

object CalDAV

The payload you use to configure a Calendar account.

object CardDAV

The payload you use to configure a Contacts account.

object GoogleAccount

The payload you use to configure a Google account.

object LDAP

The payload you use to configure an LDAP account.

object MobileAccounts

The payload you use to configure mobile accounts on the device.

object SubscribedCalendars

The payload you use to configure subscribed calendars.

### AirPlay

object AirPlay

The payload you use to configure AirPlay settings.

object AirPlaySecurity

The payload you use to configure Apple TV for a particular style of AirPlay security.

### App Management

object AppLock

The payload you use to configure a device to run a single app.

object AssociatedDomains

The payload you use to configure associated domains.

object AutonomousSingleAppMode

The payload you use to configure Autonomous Single App mode.

object NSExtensionManagement

The payload you use to configure the extensions that the system allows or disallows to run on the device.

### App Store

object AppStore

The payload you use to configure macOS App Store restrictions.

### Apple TV

object ConferenceRoomDisplay

The payload you use to configure Conference Room Display mode for Apple TV.

object TVRemote

The payload you use to configure the Apple TV remote.

### Authentication

object DirectoryService

The payload you use to configure an Active Directory (AD) domain.

object ExtensibleSingleSignOn

The payload you use to configure an app extension that performs single sign-on (SSO).

object ExtensibleSingleSignOnKerberos

The payload you use to configure an app extension that performs single sign-on with the Kerberos extension.

object Identification

The payload you use to configure the names of the account user.

object IdentityPreference

The payload you use to configure the user’s identity on the device.

object SingleSignOn

The payload you use to configure single sign-on (SSO).

### Certificates

object ACMECertificate

The payload you use to configure Automated Certificate Management Environment (ACME) Certificate settings.

object ActiveDirectoryCertificate

The payload you use to configure Active Directory Certificate settings.

object CertificatePEM

The payload you use to configure a PEM-formatted certificate.

object CertificatePKCS1

The payload you use to configure a PKCS \#1-formatted certificate.

object CertificatePKCS12

The payload you use to configure a PKCS \#12-formatted certificate.

object CertificateRoot

The payload you use to configure a root certificate.

object CertificatePreference

The payload you use to configure a certificate preference.

object CertificateRevocation

The payload you use to configure certificate revocation checking.

object CertificateTransparency

The payload you use to configure certificate transparency enforcement.

object SCEP

The payload you use to configure Simple Certificate Enrollment Protocol (SCEP).

### Ethernet

object 8021XGlobalEthernet

The payload you use to configure the default fallback global Ethernet interface.

type 8021XFirstActiveEthernet

The payload you use to configure the first wired, active Ethernet interface.

type 8021XFirstEthernet

The payload you use to configure the first wired Ethernet interface.

type 8021XSecondActiveEthernet

The payload you use to configure the second wired, active Ethernet interface.

type 8021XSecondEthernet

The payload you use to configure the second wired Ethernet interface.

type 8021XThirdActiveEthernet

The payload you use to configure the third wired, active Ethernet interface.

type 8021XThirdEthernet

The payload you use to configure the third wired Ethernet interface.

### Full Disk Encryption

object FDEFileVault

The payload you use to configure FileVault.

object FDEFileVaultOptions

The payload you use to configure FileVault options.

object FDERecoveryKeyEscrow

The payload you use to configure FileVault recovery key escrow.

### Login

object LoginItemsManagedItems

The payload you use to configure a device’s login items.

object LoginWindowLoginItems

The payload you use to configure login behavior.

object LoginWindow

The payload you use to configure login window behavior.

object LoginWindowScripts

The payload you use to configure scripts to run at login and logout.

object ServiceManagementManagedLoginItems

This payload you use to configure managed login items, which auto-enables and auto-allows matched items.

### Mail

object ExchangeActiveSync

The payload you use to configure Exchange ActiveSync accounts.

object ExchangeWebServices

The payload you use to configure an Exchange Web Services account for Contacts, Mail, Notes, Reminders, and Calendar.

object Mail

The payload you use to configure a mail account on the device.

### Managed Devices

object EducationConfiguration

The payload you use to configure the users, groups, and departments within an educational organization.

object LightsOutManagementLOM

The payload you use to configure lights-out management (LOM) settings.

object ManagedPreferences

The payload you use to configure managed preferences.

object MDM

The payload you use to configure mobile device management (MDM) settings.

object ProfileRemovalPassword

The payload you use to configure profile removal.

### Media Management

object MediaManagementDiscBurning

The payload you use to configure disc-burning settings.

### Networking

object Cellular

The payload you use to configure cellular settings.

object CellularPrivateNetwork

The payload to provide device info on private network deployments, including geographical location, preference over Wi-Fi, and network deployment type.

object ContentCaching

The payload you use to configure the content-caching service.

object DNSSettings

The payload you use to configure encrypted DNS settings.

object Domains

The payload you use to configure the domains under an organization’s management.

object Firewall

The payload you use to configure the firewall.

object NetworkUsageRules

The payload you use to configure network-usage rules.

object Relay

The payload you use to configure relay settings.

object WiFi

The payload you use to configure Wi-Fi settings.

object WiFiManagedSettings

The payload you use to configure managed Wi-Fi settings.

### Parental Controls

object ParentalControlsApplicationRestrictions

The payload you use to configure parental controls for apps.

object ParentalControlsContentFilter

The payload you use to configure the parental control web content filters.

object ParentalControlsDictionary

The payload you use to configure parental control dictionary restrictions.

object ParentalControlsGameCenter

The payload you use to configure Game Center parental controls.

object ParentalControlsTimeLimits

The payload you use to configure parental control time limits.

### Preferences

object GlobalPreferences

The payload you use to configure global preferences.

object UserPreferences

The payload you use to configure iCloud password preferences.

### Printing

object AirPrint

The payload you use to configure AirPrint printers in the user’s printer list.

object Printing

The payload you use to configure printers.

### Privacy

object PrivacyPreferencesPolicyControl

The payload you use to configure privacy preferences.

### Proxies

object DNSProxy

The payload you use to configure DNS proxies.

object GlobalHTTPProxy

The payload you use to configure a global HTTP proxy.

object NetworkProxyConfiguration

The payload you use to configure network proxies for a device.

### Restrictions

object Restrictions

The payload you use to configure restrictions on a device.

### Security

object Passcode

The payload you use to configure a passcode policy.

object SecurityPreferences

The payload you use to configure security preferences.

object SmartCard

The payload you use to configure a smart card.

### System Configuration

object Declarations

The payload to apply a set of declaration to the device through the Settings app.

object EnergySaver

The payload you use to configure energy-saver settings.

object FileProvider

The payload you use to configure file provider settings.

object Font

The payload you use to configure fonts.

object LockScreenMessage

The payload you use to configure a Lock screen message.

object Screensaver

The payload you use to configure the screen saver.

object SystemExtensions

The payload you use to configure system extensions.

object SystemLogging

The payload you use to configure system logging.

object TimeServer

The payload you use to configure the time server.

### System Policy

object SystemPolicyControl

The payload you use to configure the system policy for assessments.

object SystemPolicyKernelExtensions

The payload you use to configure the kernel extension policies.

object SystemPolicyManaged

The payload you use to configure the Finder’s contextual menu to bypass the system policy.

object SystemPolicyRule

The payload you use to configure the system policy.

### System Updates

object SoftwareUpdate

The payload you use to configure the software update policy.

object SystemMigration

The payload you use to configure system migration.

### User Experience

object Accessibility

The payload you use to configure the accessibility features of the device.

object Desktop

The payload you use to configure the desktop.

object Dock

The payload you use to configure the dock.

object Finder

The payload you use to configure Finder settings.

object HomeScreenLayout

The payload you use to configure the Home screen layout.

object ManagedMenuExtras

The payload you use to configure menu extras.

object Notifications

The payload you use to configure notifications.

object ScreensaverUser

The payload you use to configure a user’s screen-saver settings.

object SetupAssistant

The payload you use to configure setup-assistant settings.

object TimeMachine

The payload you use to configure Time Machine.

### VPN

object AppLayerVPN

The payload you use to configure add-on VPN software.

object AppToAppLayerVPNMapping

The payload you use to configure per-app VPN settings.

object VPN

The payload you use to configure a VPN.

### Web

object WebClip

The profile you use to configure web clips on the device.

object WebContentFilter

The payload you use to configure web content filters.

### Xsan

object Xsan

The payload you use to configure an Xsan client system.

object XsanPreferences

The payload you use to configure the Xsan preferences that define the volumes that automatically mount at startup.

### Deprecated

object AIMAccount

The payload you use to configure an AIM account on the device.

object APN

The payload you use to configure access point names.

object FDERecoveryKeyRedirection

The payload you use to configure FileVault recovery key redirection.

object JabberAccount

The payload you use to configure a Jabber account.

object MacOSServerAccount

The payload you use to configure a macOS server account.

object MediaManagementAllowedMedia

The payload you use to configure media management.

object ParentalControlsDashboardWidgetRestrictions

The payload you use to configure the parental control dashboard allow list.

object ParentalControlDictationAndProfanity

The payload you use to configure parental control for dictation and profanity.

object ShareKit

The payload you use to configure ShareKit.

object SystemPreferences

The payload you use to configure the preference panes.

## See Also

### Configuration Profiles

Configuring Multiple Devices Using Profiles

Create and deploy configuration profiles to users within your organization.

