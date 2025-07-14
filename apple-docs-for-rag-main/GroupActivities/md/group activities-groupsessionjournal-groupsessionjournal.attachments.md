

- Group Activities
- GroupSessionJournal
-  GroupSessionJournal.Attachments 

Structure

# GroupSessionJournal.Attachments

An asynchronous sequence that contains one or more incoming attachment containers for you to process.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct Attachments
```

## Overview

After a participant uploads a file or data, the system makes that content available on the GroupSessionJournal.Attachments asynchronous sequence of each session participant. Configure an asynchronous task to monitor this sequence and process results when they arrive.

The following example shows you how to configure this task and use it to iterate over the available items. The `journal` variable contains a previously configured GroupSessionJournal object.

```
let attachmentListener = Task {
   for await attachments in journal.attachments {
      for attachment in attachments {
         // Download and process each attachment.
      }
   }
}
```

## Topics

### Creating an iterator

func makeAsyncIterator() -> GroupSessionJournal.Attachments.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

struct Iterator

The asynchronous iterator that produces a sequence of attachments.

typealias Element

The type of element this asynchronous sequence produces.

### Type Aliases

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Downloading content from the session

var attachments: GroupSessionJournal.Attachments

The currently available attachments for you to download and incorporate into your app.

struct Attachment

A container for the data you download.

