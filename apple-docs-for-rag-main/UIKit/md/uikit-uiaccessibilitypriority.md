

- UIKit
-  UIAccessibilityPriority 

Structure

# UIAccessibilityPriority

Constants that specify priorities for accessibility announcements.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct UIAccessibilityPriority
```

## Overview

Use these constants either with the accessibilitySpeechAnnouncementPriority property of AttributedString, or with the accessibilitySpeechAnnouncementPriority (Swift) or UIAccessibilitySpeechAttributeAnnouncementPriority (Objective-C) attributed key. For example, the following code shows how to create an announcement with a high announcement priority:

```
let highPriorityAnnouncement = NSAttributedString(string: "Camera active", attributes:
[NSAttributedString.Key.accessibilitySpeechAnnouncementPriority: UIAccessibilityPriority.high])
```

## Topics

### Choosing a priority

static let high: UIAccessibilityPriority

A high-priority announcement that interrupts other speech and isn’t interruptible after it starts.

static let `default`: UIAccessibilityPriority

A default-priority announcement that interrupts existing speech, but is interruptible if a new speech utterance starts.

static let low: UIAccessibilityPriority

A low-priority announcement that the system queues and speaks after other speech utterances are complete.

### Creating a priority

init(rawValue: String)

Creates a priority structure with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

static let accessibilitySpeechPunctuation: NSAttributedString.Key

A key that indicates whether to speak punctuation.

static let accessibilitySpeechLanguage: NSAttributedString.Key

A key that indicates the language to use when speaking a string.

static let accessibilitySpeechPitch: NSAttributedString.Key

A key that indicates the pitch to apply to spoken content.

static let accessibilitySpeechQueueAnnouncement: NSAttributedString.Key

A key that indicates whether to queue an announcement behind existing speech or to interrupt it.

Deprecated

static let accessibilitySpeechIPANotation: NSAttributedString.Key

A key that indicates the pronunciation of a specific word or phrase, such as a proper name.

static let accessibilitySpeechAnnouncementPriority: NSAttributedString.Key

static let accessibilitySpeechSpellOut: NSAttributedString.Key

