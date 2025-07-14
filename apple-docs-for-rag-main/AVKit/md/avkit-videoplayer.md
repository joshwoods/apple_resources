

- AVKit
-  VideoPlayer 

Structure

# VideoPlayer

A view that displays content from a player and a native user interface to control playback.

AVKitSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
struct VideoPlayer where VideoOverlay : View
```

## Overview

```
import SwiftUI
import AVKit

struct ContentView: View {
    @State var player = AVPlayer(url: Bundle.main.url(forResource: "video2",
                                                      withExtension: "m4v")!)
    @State var isPlaying: Bool = false

    var body: some View {
        VStack {
            VideoPlayer(player: player)
                .frame(width: 320, height: 180, alignment: .center)

            Button {
                isPlaying ? player.pause() : player.play()
                isPlaying.toggle()
                player.seek(to: .zero)
            } label: {
                Image(systemName: isPlaying ? "stop" : "play")
                    .padding()
            }
        }
    }       
}
```

## Topics

### Creating a Video Player

init(player: AVPlayer?)

Creates a video-player user interface for the player object.

init(player: AVPlayer?, videoOverlay: () -> VideoOverlay)

Creates a video-player user interface for the player object.

## Relationships

### Conforms To

- Sendable
- View

