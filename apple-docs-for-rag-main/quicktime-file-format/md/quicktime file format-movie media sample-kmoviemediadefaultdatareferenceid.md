

- QuickTime File Format
- Movie media sample
-  kMovieMediaDefaultDataReferenceID 

Data field

# kMovieMediaDefaultDataReferenceID

An identifier for the data reference to use when instantiating the embedded movie for this sample.

## Overview

This atom contains a `QTAtomID` that indicates the ID of the data reference to use when instantiating the embedded movie for this sample. If this atom is not present, the data reference with an ID of `1` is used.

## See Also

### Data fields

kMovieMediaDataReference

A data reference type and a data reference.

kMovieMediaAutoPlay

A Boolean that indicates whether or not the embedded movie starts playing immediately after instantiation.

kMovieMediaLoop

An 8-byte unsigned integer that indicates how the embedded movie should loop.

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

