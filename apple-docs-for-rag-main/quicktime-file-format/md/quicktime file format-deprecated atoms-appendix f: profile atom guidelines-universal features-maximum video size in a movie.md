

- QuickTime File Format
- Deprecated atoms
- Appendix F: Profile atom guidelines
- Universal features
-  Maximum video size in a movie 

Article

# Maximum video size in a movie

## Overview

Containing profile atom  
Movie

`part-ID`  
`0x20202020` (universal feature)

`feature-code`  
`'mvsz'`

`feature-value`  
A 32-bit packed structure holding width and height of the largest bounds needed to display the movie

## Feature Values

A packed structure in a 32-bit value:

```
struct {
    unsigned integer(16) width;
    unsigned integer(16) height;
};
```

In big-endian order, the top 16 bits correspond to the width. The lower 16 bits correspond to the height.

## Writer Responsibilities

A writer of the Maximum Movie Video Size feature should record a value that is equal to or greater than the display size needed by the movie—the actual width and height needed to display the movie at its normal size, taking into account all matrices (all track matrices and the movie matrix).

A writer (such as a CE device) may choose to record a constant size based upon its current recording mode even if the actual size recorded in the movie is smaller.

## Feature Value Algorithm

This value is calculated by examining the dimensions of all visual tracks and computing the maximum combined dimensions, including the effect of track matrices and the movie matrix. For example, if two video tracks play side-by-side in the movie, and the tracks and movie all use the identity matrix, this value will be the largest of the two tracks’ heights and their combined width.

## Reader Responsibilities

A reader of this feature code should compare the recorded value with its own video size limits.

The reader should not interpret the value of this feature as the current video size. To determine the current video size, the reader should use the dimensions of all currently displaying video tracks, their matrices, and the movie matrix.

## Comments

The width and height correspond to the maximum visual area needed to display the movie.

The summarized width and height should take into account all components of all track matrices and the movie matrix. The goal is to understand the maximum contribution of all tracks to the movie’s bounds.

For the case where there is a single video track with an identity track matrix, the movie’s maximum video size feature would typically have the same value as the track’s maximum video size feature.

## See Also

### Setting features

Table of features

Maximum video bit rate

Average video bit rate

Maximum audio bit rate

Average audio bit rate

QuickTime video codec type

QuickTime audio codec type

MPEG-4 video profile

MPEG-4 video codec

MPEG-4 video object type

MPEG-4 audio codec

Maximum video size in a track

Maximum video frame rate in a single track

Average video frame rate in a single track

Video variable frame rate indication

