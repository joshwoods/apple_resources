

- TVMLKit JS
- Restrictions
-  maxTVShowRatingForCountry 

Instance Method

# maxTVShowRatingForCountry

The maximum television show rating allowed for the specified country or region.

tvOS 9.0+

``` source
String maxTVShowRatingForCountry(
    in String countryCode
);
```

## Parameters 

`countryCode`  

An object containing the valid country code. If the code is invalid, the current country or region based on location is used.

## Return Value

A string representing the maximum allowed rating for a television show in the specified country or region; for example, PG-13.

## See Also

### Retrieving Restriction Information

allowsExplicit

A boolean value that indicates whether any explicit media is allowed.

maxMovieRank

The maximum allowed ranking for a movie.

maxMovieRatingForCountry

The maximum movie rating allowed for the specified country or region.

maxTVShowRank

The maximum allowed ranking for a television show.

