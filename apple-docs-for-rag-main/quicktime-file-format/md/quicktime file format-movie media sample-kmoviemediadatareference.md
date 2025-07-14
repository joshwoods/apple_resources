

- QuickTime File Format
- Movie media sample
-  kMovieMediaDataReference 

Data field

# kMovieMediaDataReference

A data reference type and a data reference.

## Overview

The data reference type is stored as an `OSType` at the start of the atom. The data reference is stored following the data reference type. If the data reference type is URL and the data reference is for a movie on the Apple website, the contents of the atom would be `url http://www.apple.com/foo.mov`.

There may be more than one atom of this type. The first atom of this type should have an atom ID of `1`. Additional data references should be numbered sequentially.

## See Also

### Data fields

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

kMovieMediaEnableFrameStepping

A Boolean that indicates whether the embedded movie should be considered when performing step operations.

kMovieMediaBackgroundColor

A color that is used for filling the background when the movie is being instantiated or when it fails to instantiate.

kMovieMediaRegionAtom

A number of atoms, which describe how the Movie Media Handler should resize the embedded movie.

kMovieMediaRectangleAtom

Four atoms that define a rectangle.

