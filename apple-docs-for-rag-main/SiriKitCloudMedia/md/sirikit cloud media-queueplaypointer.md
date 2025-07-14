

- SiriKit Cloud Media
-  QueuePlayPointer 

Object

# QueuePlayPointer

A position within a playback queue.

SiriKit Cloud Media 1.0.2+

``` source
object QueuePlayPointer
```

## Properties

`contentIdentifier`

ContentIdentifier

The current content.

Minimum length: `1`

Maximum length: `1000`

`offsetInMillis`

`int64`

The number of milliseconds into the playback progress of the current content. It’s the point where playback resumes after pausing.

## See Also

### Creating or Updating a Playback Queue

object Queue

A sequence of media content for playback, with links to the previous and next segments of a full playback queue.

type QueueIdentifier

A stable identifier for a playback queue.

object QueueInsertPointer

Instructions for editing the current playback queue.

