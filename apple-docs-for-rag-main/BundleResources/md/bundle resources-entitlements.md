

- Bundle Resources
-  Entitlements 

Property List

# Entitlements

Key-value pairs that grant an executable permission to use a service or technology.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

## Details 

Type  

object

## Discussion

An *entitlement* is a right or privilege that grants an executable particular capabilities. For example, an app needs the HomeKit Entitlement — along with explicit user consent — to access a user’s home automation network. An app stores its entitlements as key-value pairs embedded in the code signature of its binary executable.

You configure entitlements for your app by declaring capabilities for a target in Xcode, see Capabilities. Xcode records capabilities that you add in a property list file with the `.entitlements` extension. You can also edit the entitlements file directly. When code signing your app, Xcode combines the entitlements file, information from your developer account, and other project information to apply a final set of entitlements to your app.

## Topics

### Essentials

Diagnosing Issues with Entitlements

Verify your app’s entitlements at every stage of development to track down errors during distribution.

Signing a daemon with a restricted entitlement

Wrap a daemon in an app-like structure to use an entitlement thatʼs authorized by a provisioning profile.

### Alternative marketplaces

com.apple.developer.marketplace.app-installation

The entitlement that enables an app to vend other apps as an alternative app marketplace.

### App Clips

Parent Application Identifiers Entitlement

A list of parent application identifiers for an App Clip with exactly one entry.

**Key:** com.apple.developer.parent-application-identifiers

com.apple.developer.associated-appclip-app-identifiers

A list of App Clip identifiers for an app with exactly one entry.

com.apple.developer.on-demand-install-capable

A Boolean value that indicates whether a bundle represents an App Clip.

### Authentication

AutoFill Credential Provider Entitlement

A Boolean value that indicates whether the app may, with user permission, provide user names and passwords for AutoFill in Safari and other apps.

**Key:** com.apple.developer.authentication-services.autofill-credential-provider

Sign in with Apple Entitlement

An entitlement that lets your app use Sign in with Apple.

**Key:** com.apple.developer.applesignin

### CallKit

Default Calling App

A Boolean value that indicates whether an app can be the default calling app on someone’s device.

**Key:** com.apple.developer.calling-app

### CarPlay

com.apple.developer.carplay-audio

com.apple.developer.carplay-charging

com.apple.developer.carplay-communication

com.apple.developer.carplay-maps

com.apple.developer.carplay-parking

com.apple.developer.carplay-quick-ordering

com.apple.developer.carplay-messagingDeprecated

com.apple.developer.playable-contentDeprecated

### Contacts

com.apple.developer.contacts.notes

A Boolean value that indicates whether the app may access the notes in contact entries.

### Device Management

com.apple.developer.automated-device-enrollment.add-devices

A Boolean value that indicates whether an app may add a device to Automated Device Enrollment.

### Education

ClassKit Environment Entitlement

The ClassKit development or production environment for an education app that works with the Schoolwork app.

**Key:** com.apple.developer.ClassKit-environment

com.apple.developer.automatic-assessment-configuration

A Boolean value that indicates whether an app may create an assessment session.

### Email clients

com.apple.developer.mail-client

A Boolean that indicates whether the app can act as a user’s default email client.

### Enterprise

Apple Neural Engine access

A Boolean value that indicates whether an app can use the Apple Neural Engine to speed up CoreML.

**Key:** com.apple.developer.coreml.neural-engine-access

Increased performance headroom

An entitlement that allows an app to adjust thresholds that balance thermal dissipation and performance against fan noise and other factors.

**Key:** com.apple.developer.app-compute-category

Passthrough in screen capture

A Boolean value that indicates whether an app can include passthrough in screen capture.

**Key:** com.apple.developer.screen-capture.include-passthrough

Main camera access

A Boolean value that indicates whether an app can use ARKit to access the main cameras on Apple Vision Pro.

**Key:** com.apple.developer.arkit.main-camera-access.allow

Object-tracking parameter adjustment

A Boolean value that allows an app to use ARKit to track more objects with a higher frequency.

**Key:** com.apple.developer.arkit.object-tracking-parameter-adjustment.allow

Spatial barcode and QR code scanning

A Boolean value that indicates whether an app can use ARKit to detect, position, and decode barcode and QR codes.

**Key:** com.apple.developer.arkit.barcode-detection.allow

UVC Device Access on visionOS

A Boolean value that indicates whether the app can stream USB UVC devices connected to the Developer strap.

**Key:** com.apple.developer.avfoundation.uvc-device-access

### Exposure notification

com.apple.developer.exposure-notification

A Boolean value that indicates whether the app may use exposure notification.

### Family controls

Family Controls

A Boolean value that indicates whether the app can request or revoke authorization to provide parental controls.

**Key:** com.apple.developer.family-controls

### File provider

com.apple.developer.fileprovider.testing-mode

A Boolean value that indicates whether you can place domains in testing mode.

### Games

Game Center Entitlement

A Boolean value that indicates whether users of the app may see and compare achievements on a leaderboard, invite friends, and start multiplayer games.

**Key:** com.apple.developer.game-center

### Group activities

com.apple.developer.group-session

A Boolean value that indicates whether the app may implement shared group experiences.

### Health

HealthKit Entitlement

A Boolean value that indicates whether the app may request user authorization to access health and activity data that appears in the Health app.

**Key:** com.apple.developer.healthkit

HealthKit Capabilities Entitlement

Health data types that require additional permission.

**Key:** com.apple.developer.healthkit.access

com.apple.developer.healthkit.background-delivery

A Boolean value that indicates whether observer queries receive updates while running in the background.

com.apple.developer.healthkit.recalibrate-estimates

A Boolean value that determines whether your app can recalibrate the prediction algorithm used to calculate supported sample types.

### Home automation

HomeKit Entitlement

A Boolean value that indicates whether users of the app may manage HomeKit-compatible accessories.

**Key:** com.apple.developer.homekit

Matter Allow Setup Payload

A Boolean value that allows an app to provide an optional Matter Setup payload while setting up a Matter device in an ecosystem.

**Key:** com.apple.developer.matter.allow-setup-payload

### Hypervisor

com.apple.security.hypervisor

A Boolean value that indicates whether the app creates and manages virtual machines.

com.apple.vm.hypervisor

A Boolean value that indicates whether the app creates and manages virtual machines.

Deprecated

com.apple.vm.device-access

A Boolean value that indicates whether the app captures USB devices and uses them in the guest-operating system.

com.apple.vm.networking

A Boolean that indicates whether the app manages virtual network interfaces without escalating privileges to the root user.

com.apple.security.virtualization

A Boolean value that indicates whether your app can use the Virtualization framework.

### iCloud

com.apple.developer.icloud-container-development-container-identifiers

The container identifiers for the iCloud development environment.

com.apple.developer.icloud-container-environment

The development or production environment to use for the iCloud containers.

iCloud Container Identifiers Entitlement

The container identifiers for the iCloud production environment.

**Key:** com.apple.developer.icloud-container-identifiers

iCloud Services Entitlement

The iCloud services used by the app.

**Key:** com.apple.developer.icloud-services

iCloud Key-Value Store Entitlement

The container identifier to use for iCloud key-value storage.

**Key:** com.apple.developer.ubiquity-kvstore-identifier

### Journaling Suggestions

com.apple.developer.journal.allow

The entitlement that enables an app to present the journaling suggestions picker.

### Location

com.apple.developer.location.push

An entitlement to enable a location-sharing app to query someone’s location in response to a push notification.

### Managed App Distribution

Managed App Installation UI

An entitlement you enable so your app can use Managed App Distribution.

**Key:** com.apple.developer.managed-app-distribution.install-ui

### Media

Media Device Discovery Extension

An entitlement for an app extension that adds a specific third-party media receiver to a system device-picker UI.

**Key:** com.apple.developer.media-device-discovery-extension

com.apple.developer.coremotion.head-pose

An entitlement that enables someone’s head movement to determine the orientation of spatialized sound output.

com.apple.developer.spatial-audio.profile-access

An entitlement that enables your app to use the personalized spatial audio profile.

com.apple.developer.avfoundation.multitasking-camera-access

A Boolean value that indicates whether an app may continue using the camera at the same time as another foreground app.

Deprecated

### Memory

com.apple.developer.kernel.increased-memory-limit

A Boolean value that indicates whether core features of your app may perform better with a higher memory limit on supported devices.

Extended Virtual Addressing Entitlement

A Boolean value that indicates whether the app may access an extended address space.

**Key:** com.apple.developer.kernel.extended-virtual-addressing

### Metal

com.apple.developer.sustained-execution

A Boolean value that indicates whether your app performs consistently when the system constrains it to a sustainable performance level.

### Messages

Critical Messaging

A Boolean value that indicates whether an app can use the Critical Messaging API to send SMS messages.

**Key:** com.apple.developer.messages.critical-messaging

Default Messaging App

A Boolean value that indicates whether an app can be the default messaging app on someone’s device.

**Key:** com.apple.developer.messaging-app

### MessageUI

com.apple.developer.upi-device-validation

A Boolean value that indicates whether the app can use Unified Payments Interface (UPI) device enrollment.

### Navigation

Default Navigation

A Boolean value that indicates whether an app can be the default navigation app on someone’s device.

**Key:** com.apple.developer.navigation-app

### Networking

Network Extensions Entitlement

The APIs an app can use to customize networking features.

**Key:** com.apple.developer.networking.networkextension

Personal VPN Entitlement

The API an app can use to create and control a custom system VPN configuration.

**Key:** com.apple.developer.networking.vpn.api

Associated Domains Entitlement

The associated domains for specific services, such as shared web credentials, universal links, and App Clips.

**Key:** com.apple.developer.associated-domains

com.apple.developer.networking.multicast

A Boolean value that indicates whether an app can send or receive IP multicast traffic.

com.apple.developer.associated-domains.applinks.read-write

A Boolean value that indicates whether the app can use universal links.

com.apple.developer.networking.manage-thread-network-credentials

A Boolean value that indicates whether the app can use ThreadNetwork.

5G Network Slicing App Category

The key that defines the app category entitlement to enable Cellular Network Slicing.

**Key:** com.apple.developer.networking.slicing.appcategory

5G Network Slicing Traffic Category

The key that defines the traffic category entitlement to enable Cellular Network Slicing.

**Key:** com.apple.developer.networking.slicing.trafficcategory

com.apple.developer.networking.vmnet

### Notifications

APS Environment Entitlement

The environment for push notifications.

**Key:** aps-environment

APS Environment (macOS) Entitlement

The environment for push notifications in macOS apps.

**Key:** com.apple.developer.aps-environment

com.apple.developer.usernotifications.filtering

Enable receiving notifications without displaying the notification to the user.

### Privacy

com.apple.developer.device-information.user-assigned-device-name

The entitlement for accessing the user-assigned device name instead of a generic device name.

### Push to talk

Push to Talk Entitlement

### SafetyKit

com.apple.developer.severe-vehicular-crash-event

The entitlement for accessing Crash Detection events.

### SecureElementCredential

com.apple.developer.secure-element-credential

A Boolean value that indicates whether your app can use the SecureElementCredential framework.

com.apple.developer.secure-element-credential.default-contactless-app

A Boolean value that indicates whether your app that uses the SecureElementCredential framework can become the default contactless app.

### Security

App Sandbox

Restrict access to system resources and user data in macOS apps to contain damage if an app becomes compromised.

App Sandbox Entitlement

A Boolean value that indicates whether the app may use access control technology to contain damage to the system and user data if an app is compromised.

**Key:** com.apple.security.app-sandbox

com.apple.security.network.server

A Boolean value indicating whether your app may listen for incoming network connections.

com.apple.security.network.client

A Boolean value indicating whether your app may open outgoing network connections.

Camera entitlement

A Boolean value that indicates whether the app may interact with the built-in and external cameras, and capture movies and still images.

**Key:** com.apple.security.device.camera

com.apple.security.device.microphone

A Boolean value that indicates whether the app may use the microphone.

com.apple.security.device.usb

A Boolean value indicating whether your app may interact with USB devices.

com.apple.security.print

A Boolean value indicating whether your app may print a document.

com.apple.security.device.bluetooth

A Boolean value indicating whether your app may interact with Bluetooth devices.

Address book entitlement

A Boolean value that indicates whether the app may have read-write access to contacts in the user’s address book.

**Key:** com.apple.security.personal-information.addressbook

Location entitlement

A Boolean value that indicates whether the app may access location information from Location Services.

**Key:** com.apple.security.personal-information.location

Calendars entitlement

A Boolean value that indicates whether the app may have read-write access to the user’s calendar.

**Key:** com.apple.security.personal-information.calendars

com.apple.security.files.user-selected.read-only

A Boolean value that indicates whether the app may have read-only access to files the user has selected using an Open or Save dialog.

com.apple.security.files.user-selected.read-write

A Boolean value that indicates whether the app may have read-write access to files the user has selected using an Open or Save dialog.

com.apple.security.files.downloads.read-only

A Boolean value that indicates whether the app may have read-only access to the Downloads folder.

com.apple.security.files.downloads.read-write

A Boolean value that indicates whether the app may have read-write access to the Downloads folder.

com.apple.security.assets.pictures.read-only

A Boolean value that indicates whether the app may have read-only access to the Pictures folder.

com.apple.security.assets.pictures.read-write

A Boolean value that indicates whether the app may have read-write access to the Pictures folder.

com.apple.security.assets.music.read-only

A Boolean value that indicates whether the app may have read-only access to the Music folder.

com.apple.security.assets.music.read-write

A Boolean value that indicates whether the app may have read-write access to the Music folder.

com.apple.security.assets.movies.read-only

A Boolean value that indicates whether the app may have read-only access to the Movies folder.

com.apple.security.assets.movies.read-write

A Boolean value that indicates whether the app may have read-write access to the Movies folder.

Hardened Runtime

Manage security protections and resource access for your macOS apps.

Allow execution of JIT-compiled code entitlement

A Boolean value that indicates whether the app may create writable and executable memory using the `MAP_JIT` flag.

**Key:** com.apple.security.cs.allow-jit

Allow Unsigned Executable Memory Entitlement

A Boolean value that indicates whether the app may create writable and executable memory without the restrictions imposed by using the `MAP_JIT` flag.

**Key:** com.apple.security.cs.allow-unsigned-executable-memory

Allow DYLD environment variables entitlement

A Boolean value that indicates whether the app may be affected by dynamic linker environment variables, which you can use to inject code into your app’s process.

**Key:** com.apple.security.cs.allow-dyld-environment-variables

Disable Library Validation Entitlement

A Boolean value that indicates whether the app loads arbitrary plug-ins or frameworks, without requiring code signing.

**Key:** com.apple.security.cs.disable-library-validation

Disable Executable Memory Protection Entitlement

A Boolean value that indicates whether to disable all code signing protections while launching an app, and during its execution.

**Key:** com.apple.security.cs.disable-executable-page-protection

Debugging tool entitlement

A Boolean value that indicates whether the app is a debugger and may attach to other processes or get task ports.

**Key:** com.apple.security.cs.debugger

Audio Input Entitlement

A Boolean value that indicates whether the app may record audio using the built-in microphone and access audio input using Core Audio.

**Key:** com.apple.security.device.audio-input

Photos Library Entitlement

A Boolean value that indicates whether the app has read-write access to the user’s Photos library.

**Key:** com.apple.security.personal-information.photos-library

App Groups Entitlement

A list of identifiers specifying the groups your app belongs to.

**Key:** com.apple.security.application-groups

Apple Events Entitlement

A Boolean value that indicates whether the app may prompt the user for permission to send Apple events to other apps.

**Key:** com.apple.security.automation.apple-events

Keychain Access Groups Entitlement

The identifiers for the keychain groups that the app may share items with.

**Key:** keychain-access-groups

Data Protection Entitlement

The level of data protection for sensitive user data when an app accesses it on a device.

**Key:** com.apple.developer.default-data-protection

App Attest Environment

The environment for an app that uses the App Attest service to validate itself.

**Key:** com.apple.developer.devicecheck.appattest-environment

com.apple.security.smartcard

A Boolean that indicates whether your app has access to smart card slots and smart cards.

### Sensitive content analysis

com.apple.developer.sensitivecontentanalysis.client

A code-signing entitlement that enables an app to detect nudity in images and video.

### Sensors

com.apple.developer.sensorkit.reader.allow

The necessary entitlement to access sensor data that’s required by your app’s preapproved research study.

### Siri

Siri Entitlement

A Boolean value that indicates whether the app handles Siri requests.

**Key:** com.apple.developer.siri

### StoreKit

com.apple.developer.storekit.external-link.account

A Boolean value that indicates whether your app can link to an external website for account creation or management.

com.apple.developer.storekit.external-purchase

A Boolean value that indicates whether your app can offer external purchases.

com.apple.developer.storekit.external-purchase-link

A Boolean value that indicates whether your app can include a link that directs people to a website to make an external purchase.

### System

DriverKit

Develop device drivers in macOS and iPadOS.

System Extensions

Extend the capabilities of macOS from user space.

### Translation

Translation

A Boolean value that indicates whether an app can be the default translation app on someone’s device.

**Key:** com.apple.developer.translation-app

### TV

User Management Entitlement

The entitlement for distinguishing between multiple user accounts on Apple TV.

**Key:** com.apple.developer.user-management

com.apple.developer.video-subscriber-single-sign-on

A Boolean value that indicates whether your app can use the TV Provider Authentication service.

com.apple.smoot.subscriptionservice

A Boolean value that indicates whether your app can integrate with APIs to provide different feed based content.

### Wallet

Pass Type IDs Entitlement

A list of identifiers that specify pass types that your app can access in Wallet.

**Key:** com.apple.developer.pass-type-identifiers

Merchant IDs Entitlement

A list of merchant IDs your app uses for Apple Pay support.

**Key:** com.apple.developer.in-app-payments

com.apple.developer.in-app-identity-presentment

com.apple.developer.in-app-identity-presentment.merchant-identifiers

ID Verifier - Display Only

ID Verifier - Data Transfer

### WeatherKit

WeatherKit Entitlement

A Boolean value that indicates whether the app may use WeatherKit.

**Key:** com.apple.developer.weatherkit

### Web browsers

com.apple.developer.web-browser

A Boolean that indicates whether the app can act as the user’s default web browser.

com.apple.developer.web-browser.public-key-credential

A Boolean value that lets your app make registration and assertion requests for passkeys and security keys for any relying party identifier.

com.apple.developer.browser.app-installation

The entitlement that enables a browser to install alternative-distribution apps from a website.

### Wireless interfaces

Access Wi-Fi Information Entitlement

A Boolean value indicating whether your app can access information about the connected Wi-Fi network.

**Key:** com.apple.developer.networking.wifi-info

Wireless Accessory Configuration Entitlement

A Boolean value that indicates whether your app may configure MFi Wi-Fi accessories.

**Key:** com.apple.external-accessory.wireless-configuration

Multipath Entitlement

A Boolean value indicating whether your app may use Multipath protocols to seamlessly transition between Wi-Fi and cellular networks.

**Key:** com.apple.developer.networking.multipath

Hotspot Configuration Entitlement

A Boolean value indicating whether your app can use the hotspot manager to configure Wi-Fi networks.

**Key:** com.apple.developer.networking.HotspotConfiguration

Near Field Communication Tag Reader Session Formats Entitlement

The Near Field Communication data formats an app can read.

**Key:** com.apple.developer.nfc.readersession.formats

com.apple.developer.nfc.hce

A Boolean value indicating whether your app can use the card session API.

com.apple.developer.nfc.hce.iso7816.select-identifier-prefixes

An array of identifier strings the app handles with the card session API.

com.apple.developer.nfc.hce.default-contactless-app

A Boolean value indicating whether your app can be a default app for contactless NFC with the card session API.

### Deprecated entitlements

Maps Entitlement

A Boolean value that indicates whether the app may provide directions beyond what Maps supports, such as subway routes, hiking trails, and bike paths.

**Key:** com.apple.developer.maps

Deprecated

Inter-App Audio Entitlement

A Boolean value that indicates whether the app may exchange audio with other Inter-App Audio-enabled apps.

**Key:** inter-app-audio

Deprecated

All files entitlement

A Boolean value that indicates whether the app may have access to all files.

**Key:** com.apple.security.files.all

Deprecated

### BrowserEngineKit

com.apple.developer.embedded-web-browser-engine

com.apple.developer.memory.transfer_accept

com.apple.developer.memory.transfer_send

com.apple.developer.web-browser-engine.host

com.apple.developer.web-browser-engine.networking

com.apple.developer.web-browser-engine.rendering

com.apple.developer.web-browser-engine.webcontent

### ScreenCaptureKit

Persistent Content Capture

A Boolean value that indicates whether a Virtual Network Computing (VNC) app needs persistent access to screen capture.

**Key:** com.apple.developer.persistent-content-capture

### Type Aliases

com.apple.developer.accessibility.merchant-api-control

## See Also

### Property Lists

Information Property List

A resource containing key-value pairs that identify and configure a bundle.

Privacy manifest files

Describe the data your app or third-party SDK collects and the reasons required APIs it uses.

