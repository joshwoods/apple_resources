

- Accessibility
- AccessibilityNotification
-  AccessibilityNotification.LayoutChanged 

Structure

# AccessibilityNotification.LayoutChanged

A notification that an app posts when the layout of a screen changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct LayoutChanged
```

## Overview

Optionally, include a parameter that contains the accessibility element for VoiceOver to move to after processing the notification.

## Topics

### Creating a layout change notification

init(Any?)

Creates a layout change notification.

## See Also

### Notifications

struct Announcement

A notification that an app posts when it needs to convey an announcement to an assistive app.

struct ScreenChanged

A notification that an app posts when a new view appears that occupies a major portion of the screen.

struct PageScrolled

A notification that an app posts when a scroll action completes.

