

- Media Player
- MPMovieScalingMode
-  MPMovieScalingMode.fill Deprecated

Case

# MPMovieScalingMode.fill

Scale the movie until both dimensions fit the visible bounds of the view exactly. The aspect ratio of the movie is not preserved.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
case fill
```

Deprecated

Use AVPlayerViewController in AVKit

## See Also

### Constants

case none

Do not scale the movie.

Deprecated

case aspectFit

Scale the movie uniformly until one dimension fits the visible bounds of the view exactly. In the other dimension, the region between the edge of the movie and the edge of the view is filled with a black bar. The aspect ratio of the movie is preserved.

Deprecated

case aspectFill

Scale the movie uniformly until the movie fills the visible bounds of the view. Content at the edges of the larger of the two dimensions is clipped so that the other dimension fits the view exactly. The aspect ratio of the movie is preserved.

Deprecated

