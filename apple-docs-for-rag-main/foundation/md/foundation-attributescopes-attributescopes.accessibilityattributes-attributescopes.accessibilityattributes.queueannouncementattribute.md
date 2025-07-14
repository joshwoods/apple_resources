

- Foundation
- AttributeScopes
- AttributeScopes.AccessibilityAttributes
-  AttributeScopes.AccessibilityAttributes.QueueAnnouncementAttribute 

Enumeration

# AttributeScopes.AccessibilityAttributes.QueueAnnouncementAttribute

An attribute to define if speech announcements spoken by VoiceOver should be queued behind existing speech rather than interrupting speech in progress.

FoundationAccessibilityiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum QueueAnnouncementAttribute
```

## Overview

When `true`, the announcement will be queued behind existing speech. When `false`, it will interrupt existing speech. By default, announcements interrupt existing speech.

Note

This attribute is not used on macOS

## Relationships

### Conforms To

- AttributedStringKey
- BitwiseCopyable
- Copyable
- DecodableAttributedStringKey
- EncodableAttributedStringKey
- MarkdownDecodableAttributedStringKey
- Sendable

