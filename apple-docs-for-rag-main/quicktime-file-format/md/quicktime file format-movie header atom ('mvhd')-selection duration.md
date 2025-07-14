

- QuickTime File Format
- Movie header atom ('mvhd')
-  Selection duration 

Data field

# Selection duration

The duration of the current selection in movie time scale units.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this movie header atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this movie header atom.

Flags

Three bytes of space for future movie header flags.

Creation time

A 32-bit integer that specifies the creation calendar date and time for the movie atom.

Modification time

A 32-bit integer that specifies the calendar date and time of the last change to the movie atom.

Time scale

A time value that indicates the time scale for this movie.

Duration

A time value that indicates the duration of the movie in time scale units.

Preferred rate

A 32-bit fixed-point number that specifies the rate at which to play this movie.

Preferred volume

A 16-bit fixed-point number that specifies how loud to play this movie’s sound.

Reserved

Ten bytes reserved for use by Apple.

Matrix structure

The matrix structure associated with this movie.

Preview time

The time value in the movie at which the preview begins.

Preview duration

The duration of the movie preview in movie time scale units.

Poster time

The time value of the time of the movie poster.

