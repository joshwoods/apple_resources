

- ActivityKit
- PushType
-  channel(\_:) 

Type Method

# channel(\_:)

A constant to configure a Live Activity that updates its dynamic content for broadcast channels.

iOS 18.0+iPadOS 18.0+

``` source
static func channel(_ name: String) -> PushType
```

## Overview

The channel ID is a base64-encoded string. For information on creating a channel, refer to Sending channel management requests to APNs. The code snippet below is an example of how to specify that you want to use a broadcast push channel.

```
Activity.request(attributes: attributes, 
content: content,
pushType: .channel("c29tZUNoYW5uZWw="))
```

## See Also

### Supporting ActivityKit push notifications

static var token: PushType

A constant you use to configure a Live Activity that updates its dynamic content by receiving ActivityKit push notifications.

