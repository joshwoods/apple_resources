

- Bundle Resources
- Information Property List
-  Bundle configuration 

API Collection

# Bundle configuration

Define basic characteristics of a bundle, like its name, type, and version.

## Overview

The Information Property List file associated with a bundle tells you how to interpret the bundle’s contents. The file describes fundamental features, like whether the bundle contains an app, a framework, or something else. It also includes identifying characteristics of the bundle, like an identifier, a human-readable name, and a version.

## Topics

### Categorization

CFBundlePackageType

The type of bundle.

**Name:** Bundle OS Type code

LSApplicationCategoryType

The category that best describes your app for the App Store.

**Name:** Application Category

### Identification

CFBundleIdentifier

A unique identifier for a bundle.

**Name:** Bundle identifier

WKAppBundleIdentifier

The bundle ID of the watchOS app.

WKCompanionAppBundleIdentifier

The bundle ID of the watchOS app’s companion iOS app.

### Naming

CFBundleName

A user-visible short name for the bundle.

**Name:** Bundle name

CFBundleDisplayName

The user-visible name for the bundle, used by Siri and visible on the iOS Home screen.

**Name:** Bundle display name

CFBundleSpokenName

A replacement for the app name in text-to-speech operations.

**Name:** Accessibility Bundle Name

### Bundle version

CFBundleVersion

The version of the build that identifies an iteration of the bundle.

**Name:** Bundle version

CFBundleShortVersionString

The release or version number of the bundle.

**Name:** Bundle versions string, short

CFBundleInfoDictionaryVersion

The current version of the Information Property List structure.

**Name:** InfoDictionary version

NSHumanReadableCopyright

A human-readable copyright notice for the bundle.

**Name:** Copyright (human-readable)

### Operating system version

LSMinimumSystemVersion

The minimum version of the operating system required for the app to run in macOS.

**Name:** Minimum system version

LSMinimumSystemVersionByArchitecture

The minimum version of macOS required for the app to run on a set of architectures.

**Name:** Minimum system versions, per-architecture

MinimumOSVersion

The minimum version of the operating system required for the app to run in iOS, iPadOS, tvOS, and watchOS.

LSRequiresIPhoneOS

A Boolean value indicating whether the app must run in iOS.

**Name:** Application requires iPhone environment

WKApplication

WKWatchKitApp

A Boolean value that indicates whether the bundle is a watchOS app.

### Localization

CFBundleDevelopmentRegion

The default language and region for the bundle, as a language ID.

**Name:** Localization native development region

CFBundleLocalizations

The localizations handled manually by your app.

**Name:** Localizations

CFBundleAllowMixedLocalizations

A Boolean value that indicates whether the bundle supports the retrieval of localized strings from frameworks.

**Name:** Localized resources can be mixed

TICapsLockLanguageSwitchCapable

A Boolean value that enables the Caps Lock key to switch between Latin and non-Latin input sources.

### Help

CFAppleHelpAnchor

The name of the bundle’s HTML help file.

**Name:** Help file

CFBundleHelpBookName

The name of the help file that will be opened in Help Viewer.

**Name:** Help Book identifier

CFBundleHelpBookFolder

The name of the folder containing the bundle’s help files.

**Name:** Help Book directory name

## See Also

### Core settings

User interface

Configure an app’s scenes, storyboards, icons, fonts, and other user interface elements.

App execution

Control app launch, execution, and termination.

