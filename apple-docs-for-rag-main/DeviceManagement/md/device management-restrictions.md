

- Device Management
-  Restrictions 

Device Management Profile

# Restrictions

The payload you use to configure restrictions on a device.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object Restrictions
```

## Properties

`allowAccountModification`

`boolean`

If `false`, the system disables modification of accounts such as Apple IDs and Internet-based accounts such as Mail, Contacts, and Calendar. Available in iOS 7 and later, macOS 14 and later, and watchOS 10 and later. Requires a supervised device in iOS and watchOS.

Default: `true`

`allowActivityContinuation`

`boolean`

If `false`, the system disables activity continuation. Available in iOS 8 and later, and macOS 10.15 and later. Support for this restriction on unsupervised devices and with managed Apple IDs is deprecated.

Default: `true`

`allowAddingGameCenterFriends`

`boolean`

If `false`, the system prohibits adding friends to Game Center. Available in iOS 4.2.1 and later, and macOS 10.13 and later. Requires a supervised device in iOS 13 and later.

Default: `true`

`allowAirDrop`

`boolean`

If `false`, the system disables AirDrop. Requires a supervised device. Available in iOS 7 and later, and macOS 10.13 and later.

Default: `true`

`allowAirPlayIncomingRequests`

`boolean`

If `false`, the system disables incoming AirPlay requests. Available in macOS 12.3 and later, and tvOS 10.2 and later. Requires a supervised device in tvOS.

Default: `true`

`allowAirPrint`

`boolean`

If `false`, the system disables AirPrint. Requires a supervised device. Available in iOS 11 and later.

Default: `true`

`allowAirPrintCredentialsStorage`

`boolean`

If `false`, the system disables keychain storage of user name and password for AirPrint. Requires a supervised device. Available in iOS 11 and later.

Default: `true`

`allowAirPrintiBeaconDiscovery`

`boolean`

If `false`, the system disables iBeacon discovery of AirPrint printers, which prevents spurious AirPrint Bluetooth beacons from phishing for network traffic. Requires a supervised device. Available in iOS 11 and later.

Default: `true`

`allowAppCellularDataModification`

`boolean`

If `false`, the system disables changing settings for cellular data usage for apps. Requires a supervised device. Available in iOS 7 and later.

Default: `true`

`allowAppClips`

`boolean`

If `false`, the system prevents a user from adding any App Clips, and removes any existing App Clips on the device. Requires a supervised device. Available in iOS 14.0 and later.

Default: `true`

`allowAppInstallation`

`boolean`

If `false`, the system disables the App Store, and the system removes its icon from the Home screen. Users are unable to install or update their apps. This applies to App Store apps, marketplace apps, and locally installed apps (using Configurator, Xcode, etc).

In iOS 10 and later, MDM commands can override this restriction. Available in iOS 4 and later, and watchOS 10 and later. Requires a supervised device in iOS 13 and later, and watchOS.

Default: `true`

`allowAppleIntelligenceReport`

`boolean`

If `false`, the system disables Apple Intelligence reports. Available in iOS 18.4 and later, and macOS 15.4 and later.

Default: `true`

`allowApplePersonalizedAdvertising`

`boolean`

If `false`, the system limits Apple personalized advertising. Available in iOS 14 and later, and macOS 12 and later.

Default: `true`

`allowAppRemoval`

`boolean`

If `false`, the system disables removal of apps from an iOS device. This applies to App Store apps, marketplace apps, and locally installed apps (using Configurator, Xcode, etc).

Requires a supervised device. Available in iOS 4.2.1 and later, and watchOS 10 and later.

Default: `true`

`allowAppsToBeHidden`

`boolean`

If `false`, disables the ability for the user to hide apps. It doesn’t affect the user’s ability to leave it in the App Library, while removing it from the home screen. Available in iOS 18 and later.

Default: `true`

`allowAppsToBeLocked`

`boolean`

If `false`, disables the ability for the user to lock apps. Because hiding apps also requires locking them, disallowing locking also disallows hiding. Available in iOS 18 and later.

Default: `true`

`allowARDRemoteManagementModification`

`boolean`

If `false`, the system prevents modifying the Remote Management Sharing setting in System Settings. Available in macOS 14 and later.

Default: `true`

`allowAssistant`

`boolean`

If `false`, the system disables Siri. Available in iOS 5 and later, and macOS 14 and later. Also available for user enrollment.

Default: `true`

`allowAssistantUserGeneratedContent`

`boolean`

If `false`, the system prevents Siri from querying user-generated content from the web. Requires a supervised device. Available in iOS 7 and later, and watchOS 10 and later.

Default: `true`

`allowAssistantWhileLocked`

`boolean`

If `false`, the system disables Siri when the device is locked. The system ignores this restriction if the device doesn’t have a passcode set. Available in iOS 5.1 and later. Also available for user enrollment.

Default: `true`

`allowAutoCorrection`

`boolean`

If `false`, the system disables keyboard autocorrection. Requires a supervised device. Available in iOS 8.1.3 and later.

Default: `true`

`allowAutoDim`

`boolean`

If `false`, disables auto dim on iPads with OLED displays.Requires a supervised device in iOS. Available in iOS 17.4 and later.

Default: `true`

`allowAutomaticAppDownloads`

`boolean`

If `false`, the system prevents automatic downloading of apps purchased on other devices. This setting doesn’t affect updates to existing apps. Requires a supervised device. Available in iOS 9 and later, and watchOS 10 and later.

Default: `true`

`allowAutomaticScreenSaver`

`boolean`

If `false`, the system disables Apple TV’s automatic screen saver. Available in tvOS 15.4 and later.

Default: `true`

`allowAutoUnlock`

`boolean`

If `false`, the system disallows auto unlock. Available in macOS 10.12 and later, and iOS 14.5 and later. Support for this restriction on unsupervised devices is deprecated.

Default: `true`

`allowBluetoothModification`

`boolean`

If `false`, the system prevents modification of Bluetooth settings. Requires a supervised device. Available in iOS 11 and later.

Default: `true`

`allowBluetoothSharingModification`

`boolean`

If `false`, the system prevents modifying Bluetooth settings in System Settings. Available in macOS 14 and later.

Default: `true`

`allowBookstore`

`boolean`

If `false`, the system removes the Book Store tab from the Books app. Requires a supervised device. Available in iOS 6 and later and macOS 15 and later.

Default: `true`

`allowBookstoreErotica`

`boolean`

If `false`, the system prevents the user from downloading Apple Books media that’s tagged as erotica. Available in iOS 4.0 and later, macOS 15 and later, and tvOS 17 and later. Support for this restriction on unsupervised devices is deprecated.

Default: `true`

`allowCallRecording`

`boolean`

If `false`, disables call recording. Available in iOS 18 and later.

Default: `true`

`allowCamera`

`boolean`

If `false`, the system disables the camera and removes its icon from the Home screen, and users are unable to take photographs. Available in iOS 4 and later, macOS 10.11 and later, and tvOS 17 and later. Support for this restriction on unsupervised devices is deprecated.

Default: `true`

`allowCellularPlanModification`

`boolean`

If `false`, the system prevents users from changing settings related to their cellular plan (only available on select carriers). Requires a supervised device. Available in iOS 11 and later.

Default: `true`

`allowChat`

`boolean`

If `false`, the system disables the use of iMessage with supervised devices. If the device supports text messaging, the user can still send and receive text messages. Requires a supervised device. Available in iOS 5 and later.

Default: `true`

`allowCloudAddressBook`

`boolean`

If `false`, the system disables iCloud Address Book services. Available in macOS 10.12 and later.

Default: `true`

`allowCloudBackup`

`boolean`

If `false`, the system disables backing up the device to iCloud. Available in iOS 5 and later. Support for this restriction on unsupervised devices is deprecated.

Default: `true`

`allowCloudBookmarks`

`boolean`

If `false`, the system disables iCloud Bookmark sync. Available in macOS 10.12 and later.

Default: `true`

`allowCloudCalendar`

`boolean`

If `false`, the system disables iCloud Calendar services. Available in macOS 10.12 and later.

Default: `true`

`allowCloudDesktopAndDocuments`

`boolean`

If `false`, the system disables iCloud Desktop and Document services. Available in macOS 10.12.4 and later.

Default: `true`

`allowCloudDocumentSync`

`boolean`

If `false`, the system disables document and key-value syncing to iCloud. Available in iOS 5 and later, and macOS 10.11 and later. Requires a supervised device in iOS 13 and later, and Shared iPad doesn’t support it. Support for this restriction on unsupervised devices and with managed Apple IDs is deprecated.

Default: `true`

`allowCloudFreeform`

`boolean`

If `false`, the system disallows iCloud Freeform services. Available in macOS 14 and later.

Default: `true`

`allowCloudKeychainSync`

`boolean`

If `false`, the system disables iCloud keychain synchronization. Available in iOS 7 and later, and macOS 10.12 and later. Support for this restriction on unsupervised devices and with managed Apple IDs is deprecated.

Default: `true`

`allowCloudMail`

`boolean`

If `false`, the system disables iCloud Mail services. Available in macOS 10.12 and later.

Default: `true`

`allowCloudNotes`

`boolean`

If `false`, the system disables iCloud Notes services. Available in macOS 10.12 and later.

Default: `true`

`allowCloudPhotoLibrary`

`boolean`

If `false`, the system disables iCloud Photo Library. The system removes any photos from local storage that aren’t fully downloaded from iCloud Photo Library to the device. Available in iOS 9 and later, and macOS 10.12 and later. Support for this restriction on unsupervised devices and with managed Apple IDs is deprecated.

Default: `true`

`allowCloudPrivateRelay`

`boolean`

If `false`, the system disables iCloud Private Relay. Available in iOS 15 and later, and in macOS 12 and later. Requires a supervised device in iOS. Support for this restriction on unsupervised devices and with managed Apple IDs is deprecated.

Default: `true`

`allowCloudReminders`

`boolean`

If `false`, the system disables iCloud Reminder services. Available in macOS 10.12 and later.

Default: `true`

`allowContentCaching`

`boolean`

If `false`, the system disables content caching. Available in macOS 10.13 and later.

Default: `true`

`allowContinuousPathKeyboard`

`boolean`

If `false`, the system disables QuickPath keyboard. Requires a supervised device. Available in iOS 13 and later.

Default: `true`

`allowDefaultBrowserModification`

`boolean`

If `false`, disables default browser preference modification. The MDM Settings command to set the default browser preference will still work when this is applied. Available in iOS 18.2 and later, and visionOS 2.2 and later.

Default: `true`

`allowDefaultCallingAppModification`

`boolean`

If `false`, disables default calling app preference modification. The MDM Settings command to set the default calling app preference still works when this is applied. Available in iOS 18.4 and later.

Default: `true`

`allowDefaultMessagingAppModification`

`boolean`

If `false`, disables default messaging app preference modification. The MDM Settings command to set the default messaging app preference still works when this is applied. Available in iOS 18.4 and later.

Default: `true`

`allowDefinitionLookup`

`boolean`

If `false`, the system disables definition lookup. Available in iOS 8.1.3 and later, and macOS 10.11 and later. Requires a supervised device on iOS.

Default: `true`

`allowDeviceNameModification`

`boolean`

If `false`, the system prevents the user from changing the device name. Available in iOS 9 and later, macOS 14 and later, and tvOS 11.0 and later. Requires a supervised device in iOS and tvOS.

Default: `true`

`allowDeviceSleep`

`boolean`

If `false`, the system prevents the device from automatically sleeping. Requires a supervised device. Available in tvOS 13 and later.

Default: `true`

`allowDiagnosticSubmission`

`boolean`

If `false`, the system prevents the device from automatically submitting diagnostic reports to Apple. Available in iOS 6 and later, and macOS 10.13 and later. Also available for user enrollment.

Default: `true`

`allowDiagnosticSubmissionModification`

`boolean`

If `false`, the system disables changing the diagnostic submission and app analytics settings in the Diagnostics & Usage UI in Settings. Requires a supervised device. Available in iOS 9.3.2 and later.

Default: `true`

`allowDictation`

`boolean`

If `false`, the system disallows dictation input. Available in iOS 10.3 and later, and macOS 10.13 and later. Requires a supervised device in iOS.

Default: `true`

`allowEnablingRestrictions`

`boolean`

If `false`, the system disables the Enable Restrictions option in the Restrictions UI in Settings. If `false` in iOS 12 and later, the system disables the Enable ScreenTime option in the ScreenTime UI in Settings and disables ScreenTime if already enabled. Requires a supervised device. Available in iOS 8 and later.

Default: `true`

`allowEnterpriseAppTrust`

`boolean`

If `false`, the system removes the Trust Enterprise Developer button in Settings \> General \> Profiles & Device Management, which prevents provisioning apps by universal provisioning profiles. This restriction applies to free developer accounts. However, it doesn’t apply to enterprise app developers, because they’re trusted and the system installed their apps through MDM. It also doesn’t revoke previously granted trust. Available in iOS 9 and later.

Default: `true`

`allowEnterpriseBookBackup`

`boolean`

If `false`, the system disables backup of Enterprise books. Available in iOS 8 and later. Also available for user enrollment.

Default: `true`

`allowEnterpriseBookMetadataSync`

`boolean`

If `false`, the system disables sync of Enterprise books, notes, and highlights. Available in iOS 8 and later. Also available for user enrollment.

Default: `true`

`allowEraseContentAndSettings`

`boolean`

If `false`, the system disables the Erase All Content and Settings option in the Reset UI. Available in iOS 8 and later, and macOS 12 and later. Requires a supervised device in iOS.

Default: `true`

`allowESIMModification`

`boolean`

If `false`, the system disables modifications to carrier plan related settings. Requires a supervised device. Available in iOS 11 and later.

Default: `true`

`allowESIMOutgoingTransfers`

`boolean`

If `false`, prevents the transfer of an eSIM from the device on which the restriction is installed to a different device. Requires a supervised device. Available in iOS 18 and later.

Default: `true`

`allowExplicitContent`

`boolean`

If `false`, the system hides explicit music or video content purchased from the iTunes Store. The system marks explicit content as such by content providers, such as record labels, when sold through the iTunes Store. Explicit content in the News and Podcast apps is also hidden.

Available in iOS 4.0 and later, macOS 15 and later, and tvOS 11.3 and later. Requires a supervised device in iOS 13 and later. Support for this restriction on unsupervised devices is deprecated.

Default: `true`

`allowExternalIntelligenceIntegrations`

`boolean`

If `false`, disables the use of external, cloud-based intelligence services with Siri. On iOS, this restriction is temporarily allowed on unsupervised and user enrollments. In a future release, this restriction will require supervision, and will be ignored on non-supervised devices. Available in iOS 18.2 and later, and macOS 15.2 and later.

Default: `true`

`allowExternalIntelligenceIntegrationsSignIn`

`boolean`

If `false`, forces external intelligence providers into anonymous mode. If a user is already signed in to an external intelligence provider, applying this restriction will cause them to be signed out when the next request is attempted. Available in iOS 18.2 and later, and macOS 15.2 and later.

Default: `true`

`allowFileSharingModification`

`boolean`

If `false`, the system prevents modifying File Sharing setting in System Settings. Available in macOS 14 and later.

Default: `true`

`allowFilesNetworkDriveAccess`

`boolean`

If `false`, the system prevents connecting to network drives in the Files app. Requires a supervised device. Available in iOS 13.1 and later.

Default: `true`

`allowFilesUSBDriveAccess`

`boolean`

If `false`, the system prevents connecting to any connected USB devices in the Files app. Requires a supervised device. Available in iOS 13.1 and later.

Default: `true`

`allowFindMyDevice`

`boolean`

If `false`, the system disables Find My Device in the Find My app. Requires a supervised device. Available in iOS 13 and later, and macOS 10.15 and later.

Default: `true`

`allowFindMyFriends`

`boolean`

If `false`, the system disables Find My Friends in the Find My app. Requires a supervised device. Available in iOS 13 and later, and macOS 10.15 and later.

Default: `true`

`allowFindMyFriendsModification`

`boolean`

If `false`, the system disables changes to Find My Friends. Requires a supervised device. Available in iOS 7 and later.

Default: `true`

`allowFingerprintForUnlock`

`boolean`

If `false`, the system prevents Touch ID or Face ID from unlocking a device. Available in iOS 7 and later, and macOS 10.12.4 and later. Support for this restriction on unsupervised devices is deprecated.

Default: `true`

`allowFingerprintModification`

`boolean`

If `false`, the system prevents the user from modifying Touch ID or Face ID. Available in iOS 8.3 and later, and macOS 14 and later. Requires a supervised device in iOS.

Default: `true`

`allowGameCenter`

`boolean`

If `false`, the system disables Game Center, and the system removes its icon from the Home screen. Available in iOS 6 and later, and macOS 10.13 and later. Requires a supervised device in iOS.

Default: `true`

`allowGenmoji`

`boolean`

If `false`, prohibits creating new Genmoji. Requires a supervised device. Available in iOS 18 and later.

Default: `true`

`allowGlobalBackgroundFetchWhenRoaming`

`boolean`

If `false`, the system disables global background fetch activity when an iOS phone is roaming. Available in iOS 4 and later. Support for this restriction on unsupervised devices is deprecated.

Default: `true`

`allowHostPairing`

`boolean`

If `false`, the system disables host pairing with the exception of the supervision host. If there’s no configured supervision host certificate, the system disables all pairing. Host pairing lets the administrator control if an iOS device can pair with a host Mac or PC. Requires a supervised device. Available in iOS 7 and later.

Default: `true`

`allowImagePlayground`

`boolean`

If `false`, prohibits the use of image generation. Requires a supervised device. Available in iOS 18 and later and macOS 15 and later.

Default: `true`

`allowImageWand`

`boolean`

If `false`, prohibits the use of Image Wand. Requires a supervised device. Available in iOS 18 and later.

Default: `true`

`allowInAppPurchases`

`boolean`

If `false`, the system prohibits in-app purchasing. Available in iOS 4 and later. Support for this restriction on unsupervised devices is deprecated.

Default: `true`

`allowInternetSharingModification`

`boolean`

If `false`, the system prevents modifying the Internet Sharing setting in System Settings. Available in macOS 14 and later.

Default: `true`

`allowiPhoneMirroring`

`boolean`

If `false`, prohibits the use of iPhone Mirroring. When used on macOS, this prevents the Mac from mirroring any iPhone. When used on iOS, this prevents the iPhone from mirroring to any Mac. Requires a supervised device. Available in iOS 18 and later and macOS 15 and later.

Default: `true`

`allowiPhoneWidgetsOnMac`

`boolean`

If `false`, the system disallows iPhone widgets on a Mac that has signed in the same Apple ID for iCloud. Requires a supervised device. Available on iOS 17 and later.

Default: `true`

`allowiTunes`

`boolean`

If `false`, the system disables the iTunes Music Store, and the system removes its icon from the Home screen. Users can’t preview, purchase, or download content. Available in iOS 4 and later. Requires a supervised device in iOS 13 and later.

Default: `true`

`allowiTunesFileSharing`

`boolean`

If `false`, the system disables iTunes file sharing services. Available in macOS 10.13 and later.

Default: `true`

`allowKeyboardShortcuts`

`boolean`

If `false`, the system disables keyboard shortcuts. Requires a supervised device. Available in iOS 9 and later.

Default: `true`

`allowListedAppBundleIDs`

`[string]`

If present, the system only shows or can launch apps with bundle IDs in the array. Include the value `com.apple.webapp` to allow all webclips. This applies to App Store apps, marketplace apps, and locally installed apps (using Configurator, Xcode, etc).

Requires a supervised device. Available in iOS 15 and later, and tvOS 15 and later.

`allowLiveVoicemail`

`boolean`

If `false`, the system disables live voicemail on the device.

Requires a supervised device. Available in iOS 17.2 and later.

Default: `true`

`allowLocalUserCreation`

`boolean`

If `false`, the system prevents creating new users in System Settings. Available in macOS 14 and later.

Default: `true`

`allowLockScreenControlCenter`

`boolean`

If `false`, the system prevents Control Center from appearing on the Lock screen. Available in iOS 7 and later. Also available for user enrollment.

Default: `true`

`allowLockScreenNotificationsView`

`boolean`

If `false`, the system disables the Notifications history view on the lock screen, so users can’t view past notifications. However, they can still see notifications when they arrive. Available in iOS 7 and later. Also available for user enrollment.

Default: `true`

`allowLockScreenTodayView`

`boolean`

If `false`, the system disables the Today view in Notification Center on the lock screen. Available in iOS 7 and later. Also available for user enrollment.

Default: `true`

`allowMailPrivacyProtection`

`boolean`

If `false`, the system disables Mail Privacy Protection on the device. Requires a supervised device. Available in iOS 15.2 and later.

Default: `true`

`allowMailSmartReplies`

`boolean`

If `false`, disables smart replies in Mail. Available in iOS 18.2 and later, and macOS 15.2 and later.

Default: `true`

`allowMailSummary`

`boolean`

If `false`, disables the ability to create summaries of email messages manually. This doesn’t affect automatic summary generation. Available in iOS 18.1 and later.

Default: `true`

`allowManagedAppsCloudSync`

`boolean`

If `false`, the system prevents managed apps from using iCloud sync. Available in iOS 8 and later. Also available for user enrollment.

Default: `true`

`allowManagedToWriteUnmanagedContacts`

`boolean`

If `true`, the system allows managed apps to write contacts to unmanaged accounts. If `allowOpenFromManagedToUnmanaged` is `true`, this restriction has no effect. Available in iOS 12 and later.

Important

Use MDM to install profiles that contain this restriction.

Default: `false`

`allowMarketplaceAppInstallation`

`boolean`

If `false`, the system prevents installation of alternative marketplace apps from the web and prevents any installed alternative marketplace apps from installing apps. Available in iOS 17.4 and later. Requires a supervised device

Default: `true`

`allowMediaSharingModification`

`boolean`

If `false`, prevents modification of Media Sharing settings. Available in macOS 15.1 and later.

Default: `true`

`allowMultiplayerGaming`

`boolean`

If `false`, the system prohibits multiplayer gaming. Available in iOS 4.1 and later, and macOS 10.13 and later. Requires a supervised device in iOS.

Default: `true`

`allowMusicService`

`boolean`

If `false`, the system disables the Music service, and the Music app reverts to classic mode. Requires a supervised device. Available in iOS 9.3 and later, and macOS 10.12 and later.

Default: `true`

`allowNews`

`boolean`

If `false`, the system disables News. Requires a supervised device. Available in iOS 9 and later.

Default: `true`

`allowNFC`

`boolean`

If `false`, the system disables NFC. Requires a supervised device. Available in iOS 14.2 and later.

Default: `true`

`allowNotesTranscription`

`boolean`

If `false`, disables transcription in Notes. Available in iOS 18.2 and later, and macOS 15.2 and later.

Default: `true`

`allowNotesTranscriptionSummary`

`boolean`

If `false`, disables transcription summarization in Notes. Available in iOS 18.3 and later, and macOS 15.3 and later.

Default: `true`

`allowNotificationsModification`

`boolean`

If `false`, the system disables modification of notification settings. Requires a supervised device. Available in iOS 9.3 and later.

Default: `true`

`allowOpenFromManagedToUnmanaged`

`boolean`

If `false`, documents in managed apps and accounts only open in other managed apps and accounts. Available in iOS 7 and later. Also available for user enrollment.

Default: `true`

`allowOpenFromUnmanagedToManaged`

`boolean`

If `false`, documents in unmanaged apps and accounts only open in other unmanaged apps and accounts. Available in iOS 7 and later. Also available for user enrollment.

Default: `true`

`allowOTAPKIUpdates`

`boolean`

If `false`, the system disables over-the-air PKI updates. Setting this restriction to `false` doesn’t disable CRL and OCSP checks. Available in iOS 7 and later.

Default: `true`

`allowPairedWatch`

`boolean`

If `false`, the system disables pairing with an Apple Watch, and the system unpairs any currently paired Apple Watch and erases its content. Requires a supervised device. Available in iOS 9 and later.

Default: `true`

`allowPasscodeModification`

`boolean`

If `false`, the system prevents adding, changing, or removing the passcode. The system ignores this restriction on Shared iPad. Available in iOS 9 and later, and macOS 10.13 and later. Requires a supervised device in iOS.

Default: `true`

`allowPassbookWhileLocked`

`boolean`

If `false`, the system hides Passbook notifications from the lock screen. Available in iOS 6 and later.

Default: `true`

`allowPasswordAutoFill`

`boolean`

If `false`, the system disables:

- The AutoFill Passwords feature in iOS, with Keychain and third-party password managers

- Prompting the user to use a saved password in Safari or in apps

- Automatic strong passwords

- Suggesting strong passwords to users

However, if `false`, the system doesn’t prevent AutoFill for contact info and credit cards in Safari.

Available in iOS 12 and later, and macOS 10.14 and later. Requires a supervised device in iOS.

Default: `true`

`allowPasswordProximityRequests`

`boolean`

If `false`, the system disables requesting passwords from nearby devices. Available in iOS 12 and later, macOS 10.14 and later, and tvOS 12 and later. Requires a supervised device in iOS and tvOS.

Default: `true`

`allowPasswordSharing`

`boolean`

If `false`, the system disables sharing passwords with the Airdrop Passwords feature. Available in iOS 12 and later, and macOS 10.14 and later. Requires a supervised device in iOS.

Default: `true`

`allowPersonalHotspotModification`

`boolean`

If `false`, the system disables modifications of the personal hotspot setting. Requires a supervised device. Available in iOS 12.2 and later.

Default: `true`

`allowPersonalizedHandwritingResults`

`boolean`

If false, prevents the system from generating text in the user’s handwriting. Requires a supervised device. Available in iOS 18 and later.

Default: `true`

`allowPodcasts`

`boolean`

If `false`, the system disables podcasts. Requires a supervised device. Available in iOS 8 and later.

Default: `true`

`allowPredictiveKeyboard`

`boolean`

If `false`, the system disables predictive keyboards. Requires a supervised device. Available in iOS 8.1.3 and later.

Default: `true`

`allowPrinterSharingModification`

`boolean`

If `false`, the system prevents modifying Printer Sharing settings in System Settings. Available in macOS 14 and later.

Default: `true`

`allowProximitySetupToNewDevice`

`boolean`

If `false`, disables the prompt to set up new devices that are nearby. Requires a supervised device. Available in iOS 11 and later.

Default: `true`

`allowRadioService`

`boolean`

If `false`, the system disables Apple Music Radio. Requires a supervised device. Available in iOS 9.3 and later.

Default: `true`

`allowRapidSecurityResponseInstallation`

`boolean`

If `false`, the system prohibits installation of rapid security responses. Available in iOS 16 and later, and macOS 13 and later.

Default: `true`

`allowRapidSecurityResponseRemoval`

`boolean`

If `false`, the system prohibits removal of rapid security responses. Available in iOS 16 and later, and macOS 13 and later.

Default: `true`

`allowRCSMessaging`

`boolean`

If `false`, prevents the use of RCS messaging. Available in iOS 18.1 and later.

Default: `true`

`allowRemoteAppleEventsModification`

`boolean`

If `false`, the system prevents modifying Remote Apple Events Sharing settings in System Settings. Available in macOS 14 and later.

Default: `true`

`allowRemoteAppPairing`

`boolean`

If `false`, the system disables pairing Apple TV for use with the Remote app or Control Center widget. Requires a supervised device. Available in tvOS 10.2 and later.

Default: `true`

`allowRemoteScreenObservation`

`boolean`

If `false`, the system disables remote screen observation by the Classroom app. Nest this key beneath `allowScreenShot` as a subrestriction. If `allowScreenShot` is `false`, the Classroom app doesn’t observe remote screens. Available in iOS 12 and later, and macOS 10.14.4 and later. Requires a supervised device until iOS 13 and macOS 10.15. Allowed for user enrollments in macOS 12 and later.

Default: `true`

`allowSafari`

`boolean`

If `false`, the system disables the Safari web browser app, and the system removes its icon from the Home screen. This setting also prevents users from opening web clips. As of iOS 13, requires a supervised device. Available in iOS 4 and later.

Default: `true`

`allowSafariSummary`

`boolean`

If `false`, the system disables the ability to summarize content in Safari. Available in iOS 18.2 and later, and macOS 15.2 and later.

Default: `true`

`allowSatelliteConnection`

`boolean`

If `false`, the system prohibits the connection to and use of satellite services. Available in iOS 18.2 and later.

Default: `true`

`allowScreenShot`

`boolean`

If `false`, the system disables saving a screenshot of the display and capturing a screen recording. It also disables the Classroom app from observing remote screens. Available in iOS 4 and later, and macOS 10.14.4 and later. Also available for user enrollment.

Default: `true`

`allowSharedDeviceTemporarySession`

`boolean`

If `false`, the system makes temporary sessions unavailable on Shared iPad. Available in iOS 13.4 and later.

Default: `true`

`allowSharedStream`

`boolean`

If `false`, the system disables Shared Photo Stream. Available in iOS 6 and later. Support for this restriction on unsupervised devices is deprecated.

Default: `true`

`allowSpellCheck`

`boolean`

If `false`, the system disables the keyboard spell checker. Requires a supervised device. Available in iOS 8.1.3 and later.

Default: `true`

`allowSpotlightInternetResults`

`boolean`

If `false`, the system disables Spotlight Internet search results in Siri Suggestions. Available in iOS 8 and later, and macOS 10.11 and later. Support for this restriction on unsupervised devices is deprecated.

Default: `true`

`allowStartupDiskModification`

`boolean`

If `false`, the system prevents modification of Startup Disk settings in System Settings. Available in macOS 14 and later.

Default: `true`

`allowSystemAppRemoval`

`boolean`

If `false`, the system disables the removal of system apps from the device. Requires a supervised device. Available in iOS 11 and later.

Default: `true`

`allowTimeMachineBackup`

`boolean`

If `false`, the system prevents modification of Time Machine settings in System Settings. Available in macOS 14 and later.

Default: `true`

`allowUIAppInstallation`

`boolean`

If `false`, the system disables the App Store, and the systems removes its icon from the Home screen. However, users can continue to use host apps such as iTunes or Configurator to install or update their apps.

In iOS 10 and later, MDM commands can override this restriction. Requires a supervised device. Available in iOS 9 and later, and watchOS 10 and later.

Default: `true`

`allowUIConfigurationProfileInstallation`

`boolean`

If `false`, the system prohibits the user from installing configuration profiles and certificates interactively. Available in iOS 6 and later, and macOS 13 and later. Requires a supervised device in iOS.

Default: `true`

`allowUniversalControl`

`boolean`

If `false`, the system disables Universal Control. Available in macOS 13 and later.

Default: `true`

`allowUnmanagedToReadManagedContacts`

`boolean`

If `true`, the system allows unmanaged apps to read from managed contacts accounts. If `allowOpenFromManagedToUnmanaged` is `true`, this restriction has no effect. Available in iOS 12 and later.

Important

Use MDM to install profiles that contain this restriction.

Default: `false`

`allowUnpairedExternalBootToRecovery`

`boolean`

If `true`, the system allows unpaired devices to boot devices into recovery. Requires a supervised device. Available in iOS 14.5 and later.

Default: `false`

`allowUntrustedTLSPrompt`

`boolean`

If `false`, the system automatically rejects untrusted HTTPS certificates without prompting the user. Available in iOS 5 and later.

Default: `true`

`allowUSBRestrictedMode`

`boolean`

If `false`, the system allows iOS devices to always connect to USB accessories while locked. On macOS, allows new USB and Thunderbolt accessories and SD cards to connect without authorization. If the system has Lockdown mode enabled, it ignores this value. Available in iOS 11.4.1 and later, and macOS 13 and later. Requires a supervised device in iOS.

Default: `true`

`allowVideoConferencing`

`boolean`

If `false`, the system hides the FaceTime app. Available in iOS 4 and later. Requires a supervised device in iOS 13 and later.

Default: `true`

`allowVisualIntelligenceSummary`

`boolean`

If `false`, the system disables visual intelligence summarization. Available in iOS 18.3 and later.

Default: `true`

`allowVPNCreation`

`boolean`

If `false`, the system disables the creation of VPN configurations. Requires a supervised device. Available in iOS 11 and later.

Default: `true`

`allowWallpaperModification`

`boolean`

If `false`, the system prevents changing the wallpaper. Available in iOS 9 and later, and macOS 10.13 and later. Requires a supervised device in iOS.

Default: `true`

`allowWebDistributionAppInstallation`

`boolean`

If `false`, the device prevents installation of apps directly from the web. Available in iOS 17.5 and later.

Default: `true`

`allowWritingTools`

`boolean`

If `false`, disables Apple Intelligence writing tools. Requires a supervised device. Available in iOS 18 and later and macOS 15 and later.

Default: `true`

`allowedExternalIntelligenceWorkspaceIDs`

`[string]`

An array of strings, but currently restricted to a single element. If present, Apple Intelligence only allows the given external integration workspace ID to be used, and requires a sign-in to make requests; the user will be required to sign in to integrations that support signing in. Multiple payloads combine using an intersect operation. This means the allowed set of workspace IDs can become the empty set if conflicting values are specified in multiple payloads.

`autonomousSingleAppModePermittedAppIDs`

`[string]`

If present, the system allows apps identified by the bundle IDs listed in the array to autonomously enter Single App Mode. Requires a supervised device. Available in iOS 7 and later.

`blockedAppBundleIDs`

`[string]`

If present, the system prevents showing or launching apps with bundle IDs in the array. Include the value `com.apple.webapp` to restrict all webclips. This applies to App Store apps, marketplace apps, and locally installed apps (using Configurator, Xcode, etc).

Requires a supervised device. Available in iOS 15 and later, and tvOS 15 and later.

Note

Denying system apps may disable other functionality. For example, denying the App Store app may prevent users from accepting the terms and conditions for the user-based Volume Purchase Program (VPP).

`enforcedFingerprintTimeout`

`integer`

The value, in seconds, after which the fingerprint unlock requires a password to authenticate. The default value is 48 hours. Available in macOS 12 and later.

Default: `172800`

`enforcedSoftwareUpdateDelay`

`integer`

How many days to delay a software update on the device. With this restriction in place, the user doesn’t see a software update until the specified number of days after the software update release date. The restrictions `forceDelayedAppSoftwareUpdates` and `forceDelayedSoftwareUpdates` use this value. Available in iOS 11.3 and later, macOS 10.13.4 and later, and tvOS 12.2 and later. Requires a supervised device in iOS and tvOS.

Default: `30`

Minimum: `1`

Maximum: `90`

`enforcedSoftwareUpdateMinorOSDeferredInstallDelay`

`integer`

This restriction allows the administrator to set how many days to delay a minor OS software update on the device. When this restriction is in place, the user see a software update only after the specified delay after the release of the software update. This value controls the delay for `forceDelayedSoftwareUpdates`. Available in macOS 11.3 and later.

Default: `30`

Minimum: `1`

Maximum: `90`

`enforcedSoftwareUpdateMajorOSDeferredInstallDelay`

`integer`

This restriction allows the administrator to set how many days to delay a major software upgrade on the device. When this restriction is in place, the user sees a software upgrade only after the specified delay after the release of the software upgrade. This value controls the delay for `forceDelayedMajorSoftwareUpdates`. Available in macOS 11.3 and later.

Default: `30`

Minimum: `1`

Maximum: `90`

`enforcedSoftwareUpdateNonOSDeferredInstallDelay`

`integer`

This restriction allows the administrator to set how many days to delay an app software update on the device. When this restriction is in place, the user sees a non-OS software update only after the specified delay after the release of the software. This value controls the delay for `forceDelayedAppSoftwareUpdates`. Available in macOS 11.3 and later.

Default: `30`

Minimum: `1`

Maximum: `90`

`forceAirDropUnmanaged`

`boolean`

If `true`, the system considers AirDrop to be an unmanaged drop target. Available in iOS 9 and later. Also available for user enrollment.

Default: `false`

`forceAirPlayIncomingRequestsPairingPassword`

`boolean`

If `true`, the system forces all devices sending AirPlay requests to this device to use a pairing password. Available in tvOS 6.2 and later. This key isn’t supported in tvOS 10.2 and later. Use the AirPlay Security Payload instead.

Default: `false`

`forceAirPlayOutgoingRequestsPairingPassword`

`boolean`

If `true`, the system forces all devices receiving AirPlay requests from this device to use a pairing password. Available in iOS 7.1 and later. Also available for user enrollment.

Default: `false`

`forceAirPrintTrustedTLSRequirement`

`boolean`

If `true`, the system requires trusted certificates for TLS printing communication. Requires a supervised device. Available in iOS 11 and later.

Default: `false`

`forceAssistantProfanityFilter`

`boolean`

If `true`, the system forces the use of the profanity filter assistant. Available in iOS 11 and later, and macOS 10.13 and later. Requires a supervised device in iOS.

Default: `false`

`forceAuthenticationBeforeAutoFill`

`boolean`

If `true`, the user needs to authenticate before the system can autofill passwords or credit card information in Safari and apps. If this restriction isn’t enforced, the user can toggle this feature in Settings. Only supported on devices with Face ID or Touch ID. Requires a supervised device. Available in iOS 11 and later.

Default: `false`

`forceAutomaticDateAndTime`

`boolean`

If `true`, the system enables the Set Automatically feature in Date & Time and the user can’t disable it. The system updates the device’s time zone only when the device can determine its location using a cellular connection or Wi-Fi with location services enabled. Requires a supervised device. Available in iOS 12 and later, and tvOS 12.2 and later.

Default: `false`

`forceBypassScreenCaptureAlert`

`boolean`

If `true`, then the system bypasses the presentation of a screen capture alert. Available in macOS 15.1 and later.

Default: `false`

`forceClassroomAutomaticallyJoinClasses`

`boolean`

If `true`, the system automatically gives permission to the teacher’s requests without prompting the student. Requires a supervised device. Available in iOS 11 and later, and macOS 10.14.4 and later.

Default: `false`

`forceClassroomRequestPermissionToLeaveClasses`

`boolean`

If `true`, a student enrolled in an unmanaged course through Classroom needs to request permission from the teacher to leave the course. Requires a supervised device. Available in iOS 11.3 and later, and macOS 10.14.4 and later.

Default: `false`

`forceClassroomUnpromptedAppAndDeviceLock`

`boolean`

If `true`, the system allows the teacher to lock apps or the device without prompting the student. Requires a supervised device. Available in iOS 11 and later, and macOS 10.14.4 and later.

Default: `false`

`forceClassroomUnpromptedScreenObservation`

`boolean`

If `true` and `ScreenObservationPermissionModificationAllowed` is also `true` in the Education payload, a student enrolled in a managed course through the Classroom app automatically gives permission to that course teacher’s requests to observe the student’s screen without prompting the student. Requires a supervised device. Available in iOS 11 and later, and macOS 10.14.4 and later.

Default: `false`

`forceDelayedAppSoftwareUpdates`

`boolean`

If `true`, the system delays user visibility of non-OS software updates. Requires a supervised device. Control visibility of operating system updates through `forceDelayedSoftwareUpdates`. The delay is 30 days unless you set `enforcedSoftwareUpdateDelay` to another value. Available in macOS 11 and later.

Default: `false`

`forceDelayedMajorSoftwareUpdates`

`boolean`

If `true`, the system delays user visibility of major OS updates. Available in macOS 11.3 and later.

Default: `false`

`forceDelayedSoftwareUpdates`

`boolean`

If `true`, the system delays user visibility of software updates. In macOS, the system allows seed build updates without delay. The delay is 30 days unless you set `enforcedSoftwareUpdateDelay` to another value. Available in iOS 11.3 and later, macOS 10.13 and later, and tvOS 12.2 and later. Requires a supervised device in iOS and tvOS.

Default: `false`

`forceEncryptedBackup`

`boolean`

If `true`, the system encrypts all backups. Available in iOS 4 and later. Also available for user enrollment.

Default: `false`

`forceLimitAdTracking`

`boolean`

If `true`, the system limits ad tracking. Additionally, it disables app tracking and the Allow Apps to Request to Track setting. Available in iOS 7 and later.

Default: `false`

`forceOnDeviceOnlyDictation`

`boolean`

If `true`, the system disables connections to Siri servers for the purposes of dictation. Available in iOS 14.5 and later, macOS 14 and later, and watchOS 10 and later. Also available for user enrollment.

Default: `false`

`forceOnDeviceOnlyTranslation`

`boolean`

If `true`, the device won’t connect to Siri servers for the purposes of translation. Available in iOS 15 and later. Also available for user enrollment.

Default: `false`

`forcePreserveESIMOnErase`

`boolean`

If `true`, the system preserves eSIM when it erases the device due to too many failed password attempts or the Erase All Content and Settings option in Settings \> General \> Reset. Requires a supervised device. Available in iOS 17.2 and later.

Note

The system doesn’t preserve eSIM if Find My initiates erasing the device.

Default: `false`

`forceWatchWristDetection`

`boolean`

If `true`, the system forces a paired Apple Watch to use Wrist Detection. Available in iOS 8.2 and later. Also available for user enrollment.

Default: `false`

`forceWiFiToAllowedNetworksOnly`

`boolean`

If `true`, the system limits the device to only join Wi-Fi networks set up through a configuration profile. Requires a supervised device. Available in iOS 14.5 and later.

Default: `false`

`forceWiFiPowerOn`

`boolean`

If `true`, the system prevents turning off Wi-Fi in Settings or Control Center, even by entering or leaving Airplane Mode. It doesn’t prevent selecting which Wi-Fi network to use. Requires a supervised device. Available in iOS 13.0 and later.

Default: `false`

`ratingApps`

`integer`

The maximum level of app content allowed on the device. Preinstalled (first party) apps ignore this restriction. Available in iOS 4.0 and later, macOS 15 and later, and tvOS 11.3 and later. Support for this restriction on unsupervised devices is deprecated.

Possible values, with the US description of the rating level:

- `1000`: All

- `600`: 17+

- `300`: 12+

- `200`: 9+

- `100`: 4+

- `0`: None

Default: `1000`

Minimum: `0`

Maximum: `1000`

`ratingMovies`

`integer`

The maximum level of movie content allowed on the device. Available in iOS 4.0 and later, macOS 15 and later, and tvOS 11.3 and later. Support for this restriction on unsupervised devices is deprecated.

Possible values, with the US description of the rating level:

- `1000`: All

- `500`: NC-17

- `400`: R

- `300`: PG-13

- `200`: PG

- `100`: G

- `0`: None

Default: `1000`

Minimum: `0`

Maximum: `1000`

`ratingRegion`

`string`

The two-letter key that profile tools use to display the proper ratings for the given region. The client doesn’t recognize or report this data. Available in iOS 4.0 and later, macOS 10.7 and later, and tvOS 9 and later.

Possible Values: `us, au, ca, de, fr, ie, jp, nz, gb`

`ratingTVShows`

`integer`

The maximum level of TV content allowed on the device. Available in iOS 4.0 and later, macOS 15 and later, and tvOS 11.3 and later. Support for this restriction on unsupervised devices is deprecated.

Possible values, with the US description of the rating level:

- `1000`: All

- `600`: TV-MA

- `500`: TV-14

- `400`: TV-PG

- `300`: TV-G

- `200`: TV-Y7

- `100`: TV-Y

- `0`: None

Default: `1000`

Minimum: `0`

Maximum: `1000`

`requireManagedPasteboard`

`boolean`

If `true`, copy and paste functionality conforms to the `allowOpenFromManagedToUnmanaged` and `allowOpenFromUnmanagedToManaged` restrictions. Also available for user enrollment.

Default: `false`

`safariAcceptCookies`

`number`

Defines the conditions under which the device accepts cookies. The user-facing settings changed in iOS 11, although the possible values remain the same. Available in iOS 4 and later. Support for this restriction on unsupervised devices is deprecated. Allowed values:

- `0`: Enables Prevent Cross-Site Tracking and Block All Cookies, and the user canʼt disable either setting.

- `1` or `1.5`: Enables Prevent Cross-Site Tracking, and the user canʼt disable it. Doesn’t enable Block All Cookies, but the user can enable it.

- `2`: Enables Prevent Cross-Site Tracking but doesn’t enable Block All Cookies. The user can toggle either setting.

Default: `2`

Possible Values: `0, 1, 1.5, 2`

`safariAllowAutoFill`

`boolean`

If `false`, the system disables Safari AutoFill for passwords, contact info, and credit cards and also prevents using the Keychain for AutoFill. As of iOS 13, requires a supervised device. Available in iOS 4 and later, and macOS 10.13 and later.

Note

The system still allows third-party password managers, and apps can use AutoFill.

Default: `true`

`safariAllowJavaScript`

`boolean`

If `false`, Safari doesn’t execute JavaScript. Available in iOS 4 and later.

Default: `true`

`safariAllowPopups`

`boolean`

If `false`, Safari doesn’t allow pop-up windows. Available in iOS 4 and later. Support for this restriction on unsupervised devices is deprecated.

Default: `true`

`safariForceFraudWarning`

`boolean`

If `true`, the system enables Safari fraud warning. Available in iOS 4 and later. Also available for user enrollment.

Default: `false`

`allowPhotoStream`

`boolean`

Deprecated 

If `false`, the system disables Photo Stream. Available in iOS 5 and later.

Default: `true`

`allowVoiceDialing`

`boolean`

Deprecated 

If `false`, the system disables voice dialing if the device is locked with a passcode. Available in iOS 4 and later.

Default: `true`

`blacklistedAppBundleIDs`

`[string]`

Deprecated 

Use `blockedAppBundleIDs` instead.

`forceITunesStorePasswordEntry`

`boolean`

Deprecated 

If `true`, the system forces the user to enter their iTunes password for each transaction. Available in iOS 6 and later.

Default: `false`

`whitelistedAppBundleIDs`

`[string]`

Deprecated 

Use `allowListedAppBundleIDs` instead.

`forceWiFiWhitelisting`

`boolean`

Deprecated 

Use `forceWiFiToAllowedNetworksOnly` instead.

Default: `false`

## Discussion

Specify `com.apple.applicationaccess` as the payload type.

Important

The system allows multiple Restrictions payloads. However, don’t attempt to manage the same restriction in different payloads. Doing so results in unexpected behavior.

### Profile Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | macOS, Shared iPad                     |
| Allow Manual Install       | iOS, macOS, Shared iPad, tvOS, watchOS |
| Requires Supervision       | \-                                     |
| Requires User Approved MDM | \-                                     |
| Allowed in User Enrollment | iOS, macOS, Shared iPad                |
| Allow Multiple Payloads    | iOS, macOS, Shared iPad, tvOS, watchOS |

### Profile Example

```

    PayloadContent

            allowActivityContinuation

            blockedAppBundleIDs

                com.apple.mobilesafari

            ratingApps
            500
            PayloadIdentifier
            com.example.myrestrictionspayload
            PayloadType
            com.apple.applicationaccess
            PayloadUUID
            53bec1be-ffec-4f88-acbd-b02aee8f04a9
            PayloadVersion
            1

    PayloadDisplayName
    Restrictions
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    6020206c-12c2-4ada-987a-dd4c560ca73a
    PayloadVersion
    1

```

