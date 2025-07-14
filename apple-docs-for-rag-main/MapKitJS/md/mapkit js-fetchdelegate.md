

- MapKit JS
-  FetchDelegate 

Class

# FetchDelegate

An object to pass to a map feature annotation to fetch place objects instead of a callback function.

MapKit JS 5.74+

``` source
interface FetchDelegate
```

## Overview

You can pass a `FetchDelegate` fetchPlace instead of a callback function. If you provide a delegate object, it needs to have the following methods:

- `fetchDidComplete(data)` — MapKit JS calls this method on successful completion of a fetch request. The data object is the same as the one that passes to the fetch callback function.

- `fetchDidError(error)` — MapKit JS calls this method when the fetch request fails.

## Topics

### Callback methods

fetchDidComplete

Tells the receiver when the fetch request succeeds.

fetchDidError

Tells the receiver when the fetch request fails.

## See Also

### Delegates

ImageDelegate

An object you use to specify image URLs.

