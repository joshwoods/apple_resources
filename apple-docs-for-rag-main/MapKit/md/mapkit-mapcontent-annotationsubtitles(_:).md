

- MapKit
- MapContent
-  annotationSubtitles(\_:) 

Instance Method

# annotationSubtitles(\_:)

Sets the visibility of subtitles for markers and annotations.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
func annotationSubtitles(_ visibility: Visibility) -> some MapContent
```

## Parameters 

`visibility`  

One of the `Visibility` settings. The default is Visibility.automatic, which results in the subtitle being visible only when the annotation is in a selected state.

## Return Value

Returns MapContent whose subtitles have the visibility setting you specified.

## See Also

### Supplying annotation titles

func annotationTitles(Visibility) -> some MapContent

Sets the visibility of titles for markers and annotations.

