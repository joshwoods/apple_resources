

- MapKit JS
- mapkit
-  Handling initialization events 

Article

# Handling initialization events

Respond to events that trigger when MapKit JS initializes.

## Overview

The `mapkit` object emits two events to indicate the success or failure of a configuration operation. The initialization process configures MapKit JS.

| Event | Summary |
|----|----|
| `configuration-change` | The MapKit configuration changes due to either a successful initialization or a refresh. The event has the property `status` (`String`), which indicates the configuration change status.  `Initialized`: MapKit successfully initializes and configures.  `Refreshed`: The MapKit configuration updates. |
| `error` | MapKit fails to initialize. The event has the property `status` (`String`), which indicates the status response.  `Unauthorized`: The provided authorization token is invalid.  `Too Many Requests`: The Maps ID for the authorization token provided exceeds its allowed daily usage. |

MapKit JS invokes these events asynchronously upon success or failure of the initialization request. The example below shows a common use case:

```
```

## See Also

### Initialization

init

Initializes MapKit JS by providing an authorization callback function and optional language.

MapKitInitOptions

Initialization options for MapKit JS.

Libraries

The list of available libraries.

loadedLibraries

A string that describes the list of loaded libraries.

load

Tells MapKit JS which libraries to load.

addEventListener

Subscribes a listener function to an event type.

removeEventListener

Unsubscribes a listener function from an event type.

