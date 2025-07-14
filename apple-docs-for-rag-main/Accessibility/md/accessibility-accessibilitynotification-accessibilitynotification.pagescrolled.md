

- Accessibility
- AccessibilityNotification
-  AccessibilityNotification.PageScrolled 

Structure

# AccessibilityNotification.PageScrolled

A notification that an app posts when a scroll action completes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct PageScrolled
```

## Overview

Include an announcement value, such as String or AttributedString, for an assistive app to announce. When an assistive app repeatedly receives the same scroll position value, it indicates to the user that scrolling can’t continue due to a border or boundary.

## Topics

### Creating a page scroll notification

init(String)

Creates a page scroll notification with a string.

init(AttributedString)

Creates a page scroll notification with an attributed string value.

init(NSAttributedString)

Creates a page scroll notification with an attributed string object.

## See Also

### Notifications

struct Announcement

A notification that an app posts when it needs to convey an announcement to an assistive app.

struct LayoutChanged

A notification that an app posts when the layout of a screen changes.

struct ScreenChanged

A notification that an app posts when a new view appears that occupies a major portion of the screen.

