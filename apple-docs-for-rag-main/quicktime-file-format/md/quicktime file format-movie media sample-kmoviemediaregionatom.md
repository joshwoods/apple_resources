

- QuickTime File Format
- Movie media sample
-  kMovieMediaRegionAtom 

Data field

# kMovieMediaRegionAtom

A number of atoms, which describe how the Movie Media Handler should resize the embedded movie.

## Overview

If this atom is not present, the Movie Media Handler resizes the embedded movie to completely fill the containing track’s box.

`kMovieMediaSpatialAdjustment`  
This atom contains an OSType that indicates how the embedded movie should be scaled to fit the track box. If this atom is not present, the default value is kMovieMediaFitFill. These modes are all based on SMIL layout options.

`kMovieMediaFitClipIfNecessary`  
If the media is larger than the track box, it will be clipped; if it is smaller, any additional area will be transparent.

`kMovieMediaFitFill`  
The media will be scaled to completely fill the track box.

`kMovieMediaFitMeet`  
The media is proportionally scaled so that it is entirely visible in the track box and fills the largest area possible without changing the aspect ratio.

`kMovieMediaFitSlice`  
The media is scaled proportionally so that the smaller dimension is completely visible.

`kMovieMediaFitScroll`  
Not currently implemented. It currently has the same behavior as kMovieMediaFitClipIfNecessary. When implemented, it will have the behavior described in the SMIL specification for a scrolling layout element.

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

kMovieMediaRectangleAtom

Four atoms that define a rectangle.

