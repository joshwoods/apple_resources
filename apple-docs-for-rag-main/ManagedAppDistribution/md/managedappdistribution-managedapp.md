

- ManagedAppDistribution
-  ManagedApp 

Structure

# ManagedApp

A representation of a managed app.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
struct ManagedApp
```

## Mentioned in 

Fetching and displaying managed apps

## Overview

ManagedApp represents a managed app that the framework can install. Use an instance of this object to obtain information about the app.

## Topics

### Obtaining general information

let name: String

The app’s localized name.

let subtitle: String?

The app’s localized subtitle.

let description: String?

The app’s localized description.

let fileSize: Measurement&lt;UnitInformationStorage>?

The size of the app in bytes.

func iconURL(fitting: CGSize) -> URL?

A URL for the icon of the app.

func screenshotURLs(fitting: CGSize) -> [URL]

An array of the app’s screenshot URLs.

### Obtaining platform and requirement information

let platform: Platform

The platform of the app.

let requirements: String?

The app’s localized operating system compatibility requirements.

struct Platform

The supported platform for the app.

### Obtaining supported languages

let languages: [Locale.Language]

The app’s supported languages.

let metadataLanguage: Locale.Language?

The language of the localized properties of this managed app.

### Obtaining seller information

let seller: String?

The app’s localized seller.

let developerWebsite: URL?

The app’s developer website URL.

### Obtaining rating information

let genres: [String]

The app’s localized genres.

let contentRating: String?

The app’s content age rating.

### Obtaining privacy and copyright information

let privacyPolicy: URL?

The app’s privacy policy URL.

let copyright: String?

The app’s copyright information.

var licenseAgreement: URL?

The app’s license agreement URL.

### Obtaining version information

let version: String?

The app’s version information.

let releaseNotes: String?

The app’s localized developer release notes.

let releaseDate: Date?

The app’s release date.

### Default Implementations

Equatable Implementations

Hashable Implementations

Identifiable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Identifiable
- Sendable

## See Also

### Essentials

Fetching and displaying managed apps

Provide a consistent app presentation when displaying managed apps.

class ManagedAppLibrary

A representation of a library of managed apps.

