

- QuickTime File Format
-  Movie profile atom ('prfl') Deprecated

Atom

# Movie profile atom ('prfl')

An atom that summarizes the features and complexity of a movie.

Deprecated

Profile atoms are deprecated in the QuickTime file format. The information that follows documents existing content containing profile atoms and should not be used for new development.

## Mentioned in 

QuickTime File Format change log

## Overview

The movie profile atom summarizes the features and complexity of a movie, such as the required codecs and maximum bit rate, in order to help player applications or devices quickly determine whether they have the necessary resources to play the movie.

Features for a movie typically include the movie’s maximum video and audio bit rate, a list of audio and video codec types, the movie’s video dimensions, and any applicable MPEG-4 profiles and levels. This is all information that can also be obtained by examining the contents of the movie file in more detail. This summary is intended to allow applications or devices to quickly determine whether they can play the movie. It is not intended as a container for information that is not found elsewhere in the movie, and should not be used as one.

Note

The fact that a feature does not appear in the profile atom does not mean it is not present in the movie. The profile atom itself may not be present, or may list only a subset of movie features. The features listed in the profile atom are all present, but the list is not necessarily complete.

When creating a profile atom, it is permissible to omit some features that are present in the movie, but it is required to fully specify any features that are included in the profile. For example, a movie containing video may or may not have a video codec type feature in the profile atom, but if any video codec type feature is included in the profile atom, every required video codec must be listed in the profile atom.

The movie profile atom is a profile atom (`'prfl'`) whose parent is a movie atom. This is distinct from the track profile atom, whose parent is a track atom. The structure of the profile atom is identical in both cases, but the contents of a movie profile atom describe the movie as a whole, while the contents of a track profile atom are specific to a particular track.

The profile atom contains a list of features. In a movie profile atom, these features summarize the movie as a whole. In a track profile atom, these features describe a particular track.

For details on the structure and contents of profile atoms, see Appendix F: Profile atom guidelines.

## Topics

### Data fields

Reserved

A 32-bit field.

Part-ID

A 32-bit field that defines the feature as being either brand-specific or universal.

Feature code

A 32-bit unsigned integer that represents a code specifying a feature.

Value

A 32-bit field that represents a value related to a feature.

## See Also

### Movie atoms

Track profile atom ('prfl')

A child atom of movie atoms or track atoms.

Deprecated

Appendix F: Profile atom guidelines

Summarize profile information about a QuickTime movie so readers can easily determine features and complexity.

