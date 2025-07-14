

- TVMLKit JS
-  Restrictions 

Class

# Restrictions

An object used to retrieve rating restriction information.

tvOS 9.0+

``` source
interface Restrictions
```

## Overview

Different countries often allow different levels of content to be shown. This class also allows you to specify the maximum and minimum rankings for content.

You cannot create an instance of the `Restrictions` class. An instance of this class is available from Settings.

## Topics

### Retrieving Restriction Information

allowsExplicit

A boolean value that indicates whether any explicit media is allowed.

maxMovieRank

The maximum allowed ranking for a movie.

maxMovieRatingForCountry

The maximum movie rating allowed for the specified country or region.

maxTVShowRank

The maximum allowed ranking for a television show.

maxTVShowRatingForCountry

The maximum television show rating allowed for the specified country or region.

## See Also

### Device Settings

Device

An object that provides information about an Apple TV and the host app installed on the device.

Settings

An object that provides access to setting information for a device.

