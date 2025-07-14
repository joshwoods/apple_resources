

- App Intents
-  IntentDeprecation 

Structure

# IntentDeprecation

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct IntentDeprecation where ReplacementIntent : AppIntent
```

## Topics

### Initializers

init(message: LocalizedStringResource)

init(message: LocalizedStringResource, replacedBy: ReplacementIntent.Type?)

init(replacedBy: ReplacementIntent.Type)

### Instance Properties

var message: LocalizedStringResource

A short, localized, human-readable string that describes the deprecation of this intent using sentence case and followed by a period.

var replacedBy: ReplacementIntent.Type?

Optionally, the AppIntent that replaces this one. Note: This is used by the Shortcuts app to help the user find the new AppIntent to use.

## See Also

### Supplementary content

protocol AppIntentsPackage

A type that describes app intent definitions that aren’t part of an app bundle and their dependencies.

struct IntentDescription

The human-readable description and metadata for an app intent.

struct IntentDialog

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

class IntentProjection

Projections for an app intent that returns non-optional values for parameters.

struct IntentSystemContext

Information that the system makes available to an app intent while it performs its action.

