

- MapKit JS
-  DirectionsConstructorOptions 

Structure

# DirectionsConstructorOptions

Options that you may provide when creating a directions object.

MapKit JS 5.0+

``` source
dictionary DirectionsConstructorOptions {
 string language;
};
```

## Overview

Use DirectionsConstructorOptions to set options when creating a mapkit.Directions object.

If you set `language` to a language ID, such as `fr-CA` or `en-GB`, MapKit JS returns step-by-step directions in the specified language, if available. If you don’t set `language` when initializing a mapkit.Directions object, the directions default to the language ID you provide when initializing the map with init. If the map doesn’t have a specified language upon initialization, MapKit JS returns directions in the browser’s language setting.

Set the `language` option when creating a mapkit.Directions object as in the code below:

```
var directions = new mapkit.Directions({
    language: "en-GB"
});
```

## Topics

### Initializing language

language

A language ID that determines the language for route information.

## See Also

### Creating a directions object

mapkit.Directions

Creates a directions object with options you provide.

