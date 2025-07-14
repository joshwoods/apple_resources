

- App Intents
-  Focus 

API Collection

# Focus

Adjust your app’s behavior and filter incoming notifications when the current Focus changes.

## Overview

People use Focus on macOS, iOS, and iPadOS to minimize distractions. For example, someone might use a Work Focus to hide notifications from personal email or message accounts. When someone engages a Focus, the system executes your app’s custom SetFocusFilterIntent. Define a version of this intent to update your app’s configuration and filter incoming notifications.

Related sessions from WWDC22

Session 10121: Meet Focus filters.

## Topics

### Focus filters

protocol SetFocusFilterIntent

An interface for providing an app intent that you use to adapt your app’s behavior when Focus changes.

Defining your app’s Focus filter

Customize your app’s behavior to reflect the device’s current Focus.

struct FocusFilterAppContext

A type that contains app-specific contextual information for a particular Focus, such as the notification filter criteria to apply.

struct FocusFilterSuggestionContext

A type you use to suggest app configurations for a given Focus.

### Errors

enum SetFocusFilterIntentError

Errors that can occur when you try to retrieve the current Focus configuration settings.

## See Also

### Other system experiences

Action button on iPhone and Apple Watch

Enable people to run your App Shortcuts with the Action button on iPhone or to start your app’s workout or dive sessions using the Action button on Apple Watch.

Developing a WidgetKit strategy

Explore features, tasks, related frameworks, and constraints as you make a plan to implement widgets, watch complications, and Live Activities.

