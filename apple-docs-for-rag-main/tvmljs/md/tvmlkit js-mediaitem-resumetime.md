

- TVMLKit JS
- MediaItem
-  resumeTime 

Instance Property

# resumeTime

The number of seconds from the beginning of the item at which the item begins playing.

tvOS 9.0+

``` source
attribute int resumeTime;
```

## Discussion

Use this property to begin playing a media item at a time other than at the beginning of the item. If this property contains anything other than 0, the player displays “Resume” instead of “Play from beginning” on playback.

## See Also

### Setting Timing Options

highlightGroups

An array of highlight groups, with each group containing a list of highlights.

interstitials

An array of `interstitial` objects.

