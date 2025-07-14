

- AVFoundation
- Streaming and AirPlay
-  Implementing simple enhanced buffering for your content 

Article

# Implementing simple enhanced buffering for your content

Configure your app for simple enhanced buffering to stream content faster to AirPlay-enabled devices and supported CarPlay vehicles.

## Overview

The AVPlayer and AVQueuePlayer classes provide the simplest way to enhance buffering for your content with AirPlay 2.

To implement simple enhanced buffering, complete the following steps.

1.  Create a player.

```
let player = AVQueuePlayer()
```

2.  Identify a URL that points to local or cloud content that you want to play.

3.  Create an AVAsset instance with a URL, and then create an AVPlayerItem instance with that asset.

```
let url = URL(string: "http://www.examplecontenturl.com")!
let asset = AVAsset(url: url)
let item = AVPlayerItem(asset: asset)
```

4.  Give the player item to the player.

```
player.insert(item, after: nil)
```

5.  Start playback.

```
player.play()
```

## See Also

### Buffered playback

Implementing flexible enhanced buffering for your content

Configure your app for flexible enhanced buffering to stream content faster to AirPlay-enabled devices and supported CarPlay vehicles.

Integrating AirPlay for Long-Form Video Apps

Integrate AirPlay features and implement a dedicated external playback experience by preparing the routing system for long-form video playback.

