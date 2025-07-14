

- AVKit
- AVPlayerView
-  flashChapterNumber(\_:chapterTitle:) 

Instance Method

# flashChapterNumber(\_:chapterTitle:)

Displays the chapter number and title in the player view for a brief moment.

macOS 10.9+

``` source
@MainActor
func flashChapterNumber(
    _ chapterNumber: Int,
    chapterTitle: String?
)
```

## Parameters 

`chapterNumber`  

The chapter number.

`chapterTitle`  

The chapter title. This value is optional and can be `nil`.

