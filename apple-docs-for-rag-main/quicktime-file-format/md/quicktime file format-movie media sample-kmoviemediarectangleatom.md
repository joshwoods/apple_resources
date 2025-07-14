

- QuickTime File Format
- Movie media sample
-  kMovieMediaRectangleAtom 

Data field

# kMovieMediaRectangleAtom

Four atoms that define a rectangle.

## Overview

Not all atoms must be present: top and left must both appear together, width and height must both appear together. The dimensions contained in this rectangle are used in place of the track box when applying the contents of the spatial adjustment atom. If the top and left are not specified, the top and left of the containing track’s box are used. If the width and height are not specified, the width and height of the containing track’s box are used. Each atom contains a `UInt32`.

`kMovieMediaTop`  
If present, the top of the rectangle

`kMovieMediaLeft`  
If present, the left boundary of the rectangle

`kMovieMediaWidth`  
If present, width of rectangle

`kMovieMediaHeight`  
If present, height of rectangle

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

kMovieMediaEnableFrameStepping

A Boolean that indicates whether the embedded movie should be considered when performing step operations.

kMovieMediaBackgroundColor

A color that is used for filling the background when the movie is being instantiated or when it fails to instantiate.

kMovieMediaRegionAtom

A number of atoms, which describe how the Movie Media Handler should resize the embedded movie.

