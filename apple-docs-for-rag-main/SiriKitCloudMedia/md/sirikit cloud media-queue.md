

- SiriKit Cloud Media
-  Queue 

Object

# Queue

A sequence of media content for playback, with links to the previous and next segments of a full playback queue.

SiriKit Cloud Media 1.0.2+

``` source
object Queue
```

## Properties

`content`

`[`Content`]`

 (Required) 

A sequence of songs, podcasts, ads, or other media content for the client to play.

`contentItemsCount`

`uint32`

The number of pieces of content in the full playback queue.

`controls`

QueueControlMapping

 (Required) 

The control schemes that are relevant while playing this content.

`identifier`

QueueIdentifier

 (Required) 

The identifier for the full playback queue. If you want this `Queue` to replace the client’s current playback queue, provide a new value.

Minimum length: `1`

Maximum length: `1024`

`insertPointer`

QueueInsertPointer

The position in the client’s full playback queue to insert this queue segment.

`nextContentUrl`

`string`

A URL pattern to request the next queue segment. Omit this field for the last segment in a queue, or provide a pointer to the first segment of the queue to provide a repeat mode.

Minimum length: `1`

Maximum length: `2000`

`playPointer`

QueuePlayPointer

The ContentIdentifier for the content to play next. Omit this field if you want the client to start at the beginning of the queue segment.

`prerollSeconds`

`double`

The number of seconds before the end of this queue for the client to request the next queue segment. The client may not be able to honor this hint if the user skips ahead into the last `prerollSeconds` of the current queue segment.

`previousContentUrl`

`string`

A URL pattern to request the previous queue segment. Omit this field for the first segment in a queue, or provide a pointer to the last segment of the queue to provide a repeat mode.

Minimum length: `1`

Maximum length: `2000`

`skipsRemaining`

`uint32`

For content with the `internetRadio` value in PlayMediaControlScheme, the number of times the user can skip to another track during this queue segment.

`version`

`string`

 (Required) 

The version of the `SiriKitMediaAPI` library the client uses.

Maximum length: `25`

Value: `/[0-9]+\.[0-9]+\.[0-9]+/`

## Discussion

A `Queue` object is a segment of the full playback queue. You may instruct the client to insert a `Queue` object into its current playback queue, or replace it entirely.

The strings you provide in `nextContentUrl` and `previousContentUrl` may include tokens for the client to replace at runtime. Escape the brackets delimiting the tokens as `%7B` and `%7D`. The client URL encodes its replacement values. If the client doesn’t have a current value for a token, the client replaces the token with an empty string.

The client supports the following tokens:

`{activity}`  
The `persistentIdentifier` of the client’s current UserActivity.

`{queue}`  
The QueueIdentifier for the current queue.

`{content}`  
The ContentIdentifier for the current content.

`{offset}`  
The progress, in milliseconds, within the current content.

`{firstContent}`  
The ContentIdentifier for the first item in the current queue segment.

`{lastContent}`  
The ContentIdentifier for the last item in the current queue segment.

`{transition}`  
A QueueActivityReportEvent that indicates how the client transitions to the current content.

`{version}`  
The version of the `SiriKitMediaAPI` library the client uses.

## See Also

### Creating or Updating a Playback Queue

type QueueIdentifier

A stable identifier for a playback queue.

object QueueInsertPointer

Instructions for editing the current playback queue.

object QueuePlayPointer

A position within a playback queue.

