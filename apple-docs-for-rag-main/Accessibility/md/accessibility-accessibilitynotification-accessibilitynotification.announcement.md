

- Accessibility
- AccessibilityNotification
-  AccessibilityNotification.Announcement 

Structure

# AccessibilityNotification.Announcement

A notification that an app posts when it needs to convey an announcement to an assistive app.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Announcement
```

## Overview

Include an announcement value, such as String or AttributedString, for an assistive app to announce.

Optionally, you can apply accessibility speech attributes to the announcement. For example, you can set a priority to specify the announcement’s importance relative to other announcements that are in the queue for an assistive app to speak. Announcement priorities give you more control over which announcements people need to hear, and which ones are acceptable to ignore or interrupt.

You specify an announcement priority using the accessibilitySpeechAnnouncementPriority property. The following code shows an example of how to post an announcement notification with a high priority, which interrupts other speech and isn’t interruptible after it starts:

```
```

## Topics

### Creating an announcement notification

init(String)

Creates an announcement notification with a string.

init(NSAttributedString)

Creates an announcement notification with an attributed string value.

init(AttributedString)

Creates an announcement notification with an attributed string object.

## See Also

### Notifications

struct LayoutChanged

A notification that an app posts when the layout of a screen changes.

struct ScreenChanged

A notification that an app posts when a new view appears that occupies a major portion of the screen.

struct PageScrolled

A notification that an app posts when a scroll action completes.

