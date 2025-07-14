

- QuickTime File Format
- Movie atoms
-  Interleaving movie data 

Article

# Interleaving movie data

Interleave data in your movie for optimal playback.

## Overview

In order to get optimal movie playback, you must create the movie with interleaved data. Because the data for the movie is placed on disk in time order, the data for a particular time in the movie is close together in the file. This means that you must intersperse the data from different tracks. To illustrate this, consider a movie with a single video and a single sound track.

The following figure shows how the movie data was collected, and how the data would need to be played back for proper synchronization. In this example, the video data is recorded at 10 frames per second and the audio data is grouped into half-second chunks.

After the data has been interleaved on the disk, the movie data atom would contain movie data in the order shown in the following figure.

In this example, the file begins with the movie atom (`'moov'`), followed by the movie data atom (`'mdat'`). In order to overcome any latencies in sound playback, at least one second of sound data is placed at the beginning of the interleaved data. This means that the sound and video data are offset from each other in the file by one second.

## See Also

### Describing movies

Movie atom ('moov')

An atom that specifies the information that defines a movie.

Movie header atom ('mvhd')

An atom that specifies the characteristics of an entire QuickTime movie.

Color table atom ('ctab')

An atom that defines a list of preferred colors for displaying the movie on devices that support only 256 colors.

User data atoms

Atoms you use to define and store data associated with a QuickTime object.

