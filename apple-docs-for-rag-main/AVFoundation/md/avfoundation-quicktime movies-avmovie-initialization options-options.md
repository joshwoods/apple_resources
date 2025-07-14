

- AVFoundation
- QuickTime movies
- AVMovie
-  Initialization Options 

API Collection

# Initialization Options

Specify options to configure the initialization of a movie.

## Topics

### Options

let AVMovieReferenceRestrictionsKey: String

A key that specifies restrictions for a movie to use when it resolves references to external media data.

let AVMovieShouldSupportAliasDataReferencesKey: String

A key that specifies a Boolean value that indicates whether the system parses and resolves alias data references in the movie.

## See Also

### Creating a Movie

convenience init(url: URL)

Creates a movie that models the media at the specified URL.

init(url: URL, options: [String : Any]?)

Creates a movie object from a movie header stored in a QuickTime movie file of ISO base media file.

init(data: Data, options: [String : Any]?)

Creates a movie object from a movie file’s data.

