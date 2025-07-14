

- Foundation
- AttributeScopes
- AttributeScopes.AccessibilityAttributes
- AttributeScopes.AccessibilityAttributes.AnnouncementPriorityAttribute
-  AttributeScopes.AccessibilityAttributes.AnnouncementPriorityAttribute.AnnouncementPriority 

Enumeration

# AttributeScopes.AccessibilityAttributes.AnnouncementPriorityAttribute.AnnouncementPriority

A priority level used by accessibility clients, such as VoiceOver, to control how announcements are queued and presented.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum AnnouncementPriority
```

## Topics

### Enumeration Cases

case `default`

Announcements will interrupt existing speech, but are interruptible if a new speech utterance is started.

case high

Announcements will interrupt other speech and cannot be interrupted once started.

case low

Announcements are queued and spoken when other speech utterances have completed.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

