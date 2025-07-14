

- App Intents
- AppIntent
-  title 

Type Property

# title

A short, localized, human-readable string that describes the app intent using a verb and a noun in title case.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var title: LocalizedStringResource { get }
```

**Required** Default implementation provided.

## Mentioned in 

Responding to the Action button on Apple Watch Ultra

Creating your first app intent

## Default Implementations

### AppIntent Implementations

static var title: LocalizedStringResource

A short, localized, human-readable string that describes the app intent using a verb and a noun in title case.

## See Also

### Configuring the metadata

static var description: IntentDescription?

A description of the app intent that the system shows to people.

**Required** Default implementation provided.

static var openAppWhenRun: Bool

A boolean property that tells the system to consider the app intent even if its app is not in the foreground.

**Required** Default implementations provided.

static var isDiscoverable: Bool

A boolean value that determines whether system features such as Shortcuts and Spotlight can discover this app intent.

**Required** Default implementation provided.

