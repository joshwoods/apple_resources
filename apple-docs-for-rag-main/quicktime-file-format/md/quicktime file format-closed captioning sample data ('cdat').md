

- QuickTime File Format
-  Closed captioning sample data ('cdat') 

Atom

# Closed captioning sample data ('cdat')

A sequence of one or more atoms that store closed captioning sample data.

## Overview

The format of the closed captioning sample data is a sequence of one or more atoms, one of which must be a `'cdat'` atom. Unrecognized atoms should be ignored.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this closed captioning media data atom.

Type

A 32-bit integer that identifies the atom type.

Sample data

An array of one or more byte pairs for data channel 1/field 1 (“CC1”) of a CEA-608 data stream, each byte pair corresponding to a video frame.

## See Also

### Storing closed captioning

Closed captioning sample description

An atom that defines how to interpret closed captioning media data.

Including multiple closed-caption tracks

Include multiple closed-caption tracks in a movie.

