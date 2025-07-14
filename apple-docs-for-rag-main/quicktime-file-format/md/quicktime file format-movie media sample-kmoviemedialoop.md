

- QuickTime File Format
- Movie media sample
-  kMovieMediaLoop 

Data field

# kMovieMediaLoop

An 8-byte unsigned integer that indicates how the embedded movie should loop.

## Overview

This atom is only used if the `TimeBase` of the embedded movie is not dependent on the container movie. If this atom contains a `0`, or if this atom is not present, the embedded movie will not loop. If this atom contains a value of `1`, the embedded movie loops normally — that is, when it reaches the end it loops back to the beginning. If this atom contains a value of `2`, the embedded movie uses palindromic looping. All other values are reserved.

## See Also

### Data fields

kMovieMediaDataReference

A data reference type and a data reference.

kMovieMediaDefaultDataReferenceID

An identifier for the data reference to use when instantiating the embedded movie for this sample.

kMovieMediaAutoPlay

A Boolean that indicates whether or not the embedded movie starts playing immediately after instantiation.

kMovieMediaUseMIMEType

Text (not a C string or a pascal string) that indicates the MIME type of the movie import component that should be used to instantiate this media.

kMovieMediaTitle

Currently unused.

kMovieMediaAltText

Text (not a C string or a pascal string) that is displayed to the user when the embedded movie is being instantiated or if the embedded movie cannot be instantiated.

kMovieMediaClipBegin

A record that indicates the time of the embedded movie to use.

kMovieMediaClipDuration

A record that indicates the duration of the embedded movie to use.

kMovieMediaEnableFrameStepping

A Boolean that indicates whether the embedded movie should be considered when performing step operations.

kMovieMediaBackgroundColor

A color that is used for filling the background when the movie is being instantiated or when it fails to instantiate.

kMovieMediaRegionAtom

A number of atoms, which describe how the Movie Media Handler should resize the embedded movie.

kMovieMediaRectangleAtom

Four atoms that define a rectangle.

