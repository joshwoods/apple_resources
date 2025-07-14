

- AVFoundation
- AVFragmentedMovieMinder
-  init(movie:mindingInterval:) 

Initializer

# init(movie:mindingInterval:)

Creates a movie minder and adds a movie with a minding interval.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
init(
    movie: AVFragmentedMovie,
    mindingInterval: TimeInterval
)
```

## Parameters 

`movie`  

The fragmented movie object added to the movie minder.

`mindingInterval`  

The initial minding interval for the movie minder.

## Return Value

A new `AVFragmentedMovieMinder` instance.

