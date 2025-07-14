

- Apple News API
-  Channel 

Object

# Channel

See the fields the read channel endpoint returned.

Apple News API 1.0+

``` source
object Channel
```

## Properties

`createdAt`

`date-time`

The date and time the channel was created.

`fonts`

`[string]`

The list of custom fonts used in the channel. This list may be empty.

`id`

`uuid`

The unique identifier of the channel.

`modifiedAt`

`date-time`

The date and time the channel was last modified.

`name`

`string`

The name of the channel.

`shareUrl`

`string`

The URL to the channel within the News app.

`type`

`string`

The channel.

`website`

`string`

The website that corresponds to this channel.

## Mentioned in 

Signing the HTTP Request

## Relationships

### Inherited By

- ChannelResponse

## See Also

### Channel

Read Channel Information

Get details about your channel, including the name, corresponding website, and default section.

Read Channel Quota Information

Get details about your channel’s remaining quota for sending create and update requests, the queue size, and wait time.

object ChannelLinks

See the links the read channel endpoint returned.

object ChannelResponse

See which objects make up the channel response.

