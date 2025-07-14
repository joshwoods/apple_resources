

- SiriKit Cloud Media
-  QueueInsertPointer 

Object

# QueueInsertPointer

Instructions for editing the current playback queue.

SiriKit Cloud Media 1.0.2+

``` source
object QueueInsertPointer
```

## Properties

`afterIdentifier`

ContentIdentifier

The client inserts the new queue segment after the content with this identifier.

Minimum length: `1`

Maximum length: `1000`

`replace`

`boolean`

If this value is `true`, the client discards all of the current queue’s content after the item that `afterIdentifier` specifies.

Default: `false`

## See Also

### Creating or Updating a Playback Queue

object Queue

A sequence of media content for playback, with links to the previous and next segments of a full playback queue.

type QueueIdentifier

A stable identifier for a playback queue.

object QueuePlayPointer

A position within a playback queue.

