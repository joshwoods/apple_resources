

- ManagedSettings
- MediaSettings
-  maximumMovieRating 

Type Property

# maximumMovieRating

The metadata for the setting that controls the maximum movie rating.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static let maximumMovieRating: BoundedSettingMetadata
```

## Discussion

The default value is `1000` and the bounds are `0...1000`.

## See Also

### Limiting Movie and TV Show Ratings

var maximumMovieRating: Int?

The maximum movie rating the user may view.

var maximumTVShowRating: Int?

The maximum TV show rating that the user may view.

static let maximumTVShowRating: BoundedSettingMetadata&lt;Int>

The metadata for the setting that controls the maximum TV show rating.

