

- App Intents
- AppIntent
-  isDiscoverable 

Type Property

# isDiscoverable

A boolean value that determines whether system features such as Shortcuts and Spotlight can discover this app intent.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var isDiscoverable: Bool { get }
```

**Required** Default implementation provided.

## Discussion

App Intents must be discoverable to support App Shortcuts. If your app intent isn’t discoverable, people can use it only when it’s directly connected by a button in a SwiftUI app or a widget.

This property is `true` by default.

## Default Implementations

### AppIntent Implementations

static var isDiscoverable: Bool

A boolean value that determines whether system features such as Shortcuts and Spotlight can discover this app intent.

## See Also

### Configuring the metadata

static var title: LocalizedStringResource

A short, localized, human-readable string that describes the app intent using a verb and a noun in title case.

**Required** Default implementation provided.

static var description: IntentDescription?

A description of the app intent that the system shows to people.

**Required** Default implementation provided.

static var openAppWhenRun: Bool

A boolean property that tells the system to consider the app intent even if its app is not in the foreground.

**Required** Default implementations provided.

