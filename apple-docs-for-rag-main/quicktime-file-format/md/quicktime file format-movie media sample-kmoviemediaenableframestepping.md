

- QuickTime File Format
- Movie media sample
-  kMovieMediaEnableFrameStepping 

Data field

# kMovieMediaEnableFrameStepping

A Boolean that indicates whether the embedded movie should be considered when performing step operations.

## Overview

This is specifically using the interesting time calls with the `nextTimeStep` flag. If this atom is not present or is set to false, the embedded movie is not included in step calculations. If the atom is set to true, it is included in step calculations.

## See Also

### Data fields

kMovieMediaDataReference

A data reference type and a data reference.

kMovieMediaDefaultDataReferenceID

An identifier for the data reference to use when instantiating the embedded movie for this sample.

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

kMovieMediaBackgroundColor

A color that is used for filling the background when the movie is being instantiated or when it fails to instantiate.

kMovieMediaRegionAtom

A number of atoms, which describe how the Movie Media Handler should resize the embedded movie.

kMovieMediaRectangleAtom

Four atoms that define a rectangle.

