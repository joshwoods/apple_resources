

- Foundation
- AttributeScopes
- AttributeScopes.AccessibilityAttributes
-  AttributeScopes.AccessibilityAttributes.AnnouncementPriorityAttribute 

Enumeration

# AttributeScopes.AccessibilityAttributes.AnnouncementPriorityAttribute

An attribute to define the urgency of the announcement.

FoundationAccessibilityiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@frozen
enum AnnouncementPriorityAttribute
```

## Overview

For example, when `low` is specified, announcements are queued and spoken when other speech utterances have completed. When `default` is specified, announcements will interrupt existing speech, but are interruptible if a new speech utterance is started. When `high` is specified, announcements will interrupt other speech and cannot be interrupted once started.

## Topics

### Enumerations

enum AnnouncementPriority

A priority level used by accessibility clients, such as VoiceOver, to control how announcements are queued and presented.

## Relationships

### Conforms To

- AttributedStringKey
- BitwiseCopyable
- Copyable
- DecodableAttributedStringKey
- EncodableAttributedStringKey
- MarkdownDecodableAttributedStringKey
- ObjectiveCConvertibleAttributedStringKey
- Sendable

