

- QuickTime File Format
-  Media atoms 

API Collection

# Media atoms

Atoms that describe and define a track’s media type and sample data.

## Overview

The media atom contains information that specifies:

- The media type, such as sound, video or timed metadata

- The media handler component used to interpret the sample data

- The media timescale and track duration

- Media-and-track-specific information, such as sound volume or graphics mode

- The media data references, which typically specify the file where the sample data is stored

- The sample table atoms, which, for each media sample, specify the sample description, duration, and byte offset from the data reference

## Topics

### Describing media

Media atom ('mdia')

An atom that describes and defines a track’s media type and sample data.

Media header atom ('mdhd')

An atom that specifies the characteristics of a media, including time scale and duration.

Extended language tag atom ('elng')

An atom that represents media language information.

Handler reference atom ('hdlr')

An atom that specifies the media handler component that is to be used to interpret the media’s data.

Media information atoms

An atom that contains a number of other atoms that define specific characteristics of the video media data.

Video media information atom ('minf')

An atom that contains a number of other atoms that define specific characteristics of the video media data.

Video media information header atom ('vmhd')

An atom that defines specific color and graphics mode information.

Sound media information atom ('minf')

An atom that contains a number of other atoms that define specific characteristics of the sound media data.

Sound media information header atom ('smhd')

An atom that stores the sound media’s control information, such as balance.

Base media information atom ('minf')

An atom that stores the media information for media types such as timed metadata, text, MPEG, time code, and music.

Base media information header atom ('gmhd')

An atom that indicates that this media information atom pertains to a base media.

Base media info atom ('gmin')

An atom that defines the media’s control information, including graphics mode and balance information.

Data information atom ('dinf')

An atom that specifies the data handler component that provides access to the media data.

Media data reference atom ('dref')

An atom that contains tabular data that instructs the data handler component how to access the media’s data.

## See Also

### Movies

Movie atoms

Atoms that act as a container for the information that describes a movie’s data.

Track atoms

Atoms that define a single track of a movie.

Sample atoms

Atoms that describe samples, which are single elements in a sequence of time-ordered data.

Structuring movie data and features

Build movies with compressed or reference data, and add features like effect descriptions and alternate subtitle tracks.

