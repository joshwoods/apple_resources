

- AVFoundation
- AVFragmentedMovieMinder
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes a fragmented movie from the array of movies being minded.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 6.0+

``` source
func remove(_ movie: AVFragmentedMovie)
```

## Parameters 

`movie`  

The fragmented movie removed from the minder.

## See Also

### Adding and Removing Movies

var movies: [AVFragmentedMovie]

An array containing the fragmented movie objects being minded.

func add(AVFragmentedMovie)

Adds a fragmented movie to the array of movies being minded.

