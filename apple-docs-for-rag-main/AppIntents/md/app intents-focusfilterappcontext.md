

- App Intents
-  FocusFilterAppContext 

Structure

# FocusFilterAppContext

A type that contains app-specific contextual information for a particular Focus, such as the notification filter criteria to apply.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct FocusFilterAppContext
```

## Topics

### Creating the app context

init(notificationFilterPredicate: NSPredicate?)

Creates a `FocusFilterAppContext` with a specified `notificationFilterPredicate`

### Getting the filter predicate

let notificationFilterPredicate: NSPredicate?

An `NSPredicate` for system to filter the user’s notifications of the app when a Focus is active.

### Initializers

init(notificationFilterPredicate: NSPredicate?, targetContentIdentifierPrefix: String?)

Creates a focus filter context with a specified predicate and identifier prefix.

### Instance Properties

let targetContentIdentifierPrefix: String?

An identifier you provide to the system for use in scheme prefixes for Focus.

## See Also

### Focus filters

protocol SetFocusFilterIntent

An interface for providing an app intent that you use to adapt your app’s behavior when Focus changes.

Defining your app’s Focus filter

Customize your app’s behavior to reflect the device’s current Focus.

struct FocusFilterSuggestionContext

A type you use to suggest app configurations for a given Focus.

