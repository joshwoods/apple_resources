

- MusicKit
- MusicPlayer
-  endSeeking() 

Instance Method

# endSeeking()

Ends forward and backward seeking through the music content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 14.0+tvOS 15.0+visionOS 1.0+

``` source
func endSeeking()
```

## Discussion

Call this method to end a seek operation that begins when you call either the beginSeekingBackward() or beginSeekingForward() method. After calling this method, the player returns to its previous state. For example, if the entry is playing before seeking begins, it continues playing from the new playhead position after calling this method.

