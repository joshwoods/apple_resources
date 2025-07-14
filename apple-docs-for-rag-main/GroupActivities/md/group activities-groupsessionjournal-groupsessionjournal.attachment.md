

- Group Activities
- GroupSessionJournal
-  GroupSessionJournal.Attachment 

Structure

# GroupSessionJournal.Attachment

A container for the data you download.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct Attachment
```

## Mentioned in 

Synchronizing data during a SharePlay activity

## Overview

When your app receives a new item, the system packages it in an GroupSessionJournal.Attachment and delivers it to your app. Use this container type to download the contents of the file and decode it to a type that your app recognizes.

## Topics

### Downloading the attachment data

func load&lt;AttachmentType>(AttachmentType.Type) async throws -> AttachmentType

Downloads the attachment data and asynchronously delivers it as the type you specify.

func loadMetadata&lt;MetadataType>(of: MetadataType.Type) async throws -> MetadataType

Downloads the metadata for the attachment asynchronously and delivers it as the type you specify.

### Identifying the attachment

var id: UUID

The unique identifier for this attachment.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Identifiable
- Sendable

## See Also

### Downloading content from the session

var attachments: GroupSessionJournal.Attachments

The currently available attachments for you to download and incorporate into your app.

struct Attachments

An asynchronous sequence that contains one or more incoming attachment containers for you to process.

