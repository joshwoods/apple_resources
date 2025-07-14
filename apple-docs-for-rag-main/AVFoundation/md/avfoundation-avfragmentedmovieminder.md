

- AVFoundation
-  AVFragmentedMovieMinder 

Class

# AVFragmentedMovieMinder

An object that checks whether a fragmented movie appends additional movie fragments.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
class AVFragmentedMovieMinder
```

## Overview

This class is identical to AVFragmentedAssetMinder except that it’s capable of minding only assets of type AVFragmentedMovie.

## Topics

### Creating a Movie Minder

init(movie: AVFragmentedMovie, mindingInterval: TimeInterval)

Creates a movie minder and adds a movie with a minding interval.

### Adding and Removing Movies

var movies: [AVFragmentedMovie]

An array containing the fragmented movie objects being minded.

func add(AVFragmentedMovie)

Adds a fragmented movie to the array of movies being minded.

func remove(AVFragmentedMovie)

Removes a fragmented movie from the array of movies being minded.

### Accessing Minder Information

var mindingInterval: TimeInterval

The amount of time between checks for additional movie fragments.

## Relationships

### Inherits From

- AVFragmentedAssetMinder

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Fragmented movies

class AVFragmentedMovie

An object that represents a fragmented movie file.

class AVFragmentedMovieTrack

An object that represents a track in a fragmented movie.

protocol AVFragmentMinding

A protocol that defines whether an asset supports fragment minding.

