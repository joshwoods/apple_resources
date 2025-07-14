

- MapKit JS
- mapkit
-  init 

Instance Method

# init

Initializes MapKit JS by providing an authorization callback function and optional language.

MapKit JS 5.0+

``` source
void init(
 MapKitInitOptions options
);
```

## Parameters 

`options`  

MapKit JS initialization options.

## Mentioned in 

Loading the latest version of MapKit JS

## Discussion

Unless you wish to explicitly control initialization timing in JavaScript, use `data-token` instead of this method. See Loading the latest version of MapKit JS for more information.

If you’re using this method, provide the token by setting authorizationCallback on a JavaScript object as a function. The authorizationCallback function calls `done()` to return the token. Creating a Maps token shows how to create Maps tokens.

When you create a server endpoint to deliver new tokens to MapKit JS, make an asynchronous request to this endpoint in your authorizationCallback function and call `done()` with the result. The following example shows creating a callback that requests a token from a server endpoint and sets a preferred language for the map:

```
mapkit.init({
    authorizationCallback: function(done) {
        fetch("/gettoken")
            .then(res => res.text())
            .then(done);
    },
    language: "es"
});
```

If you don’t set up a server endpoint, you can alternatively set authorizationCallback to a function that provides a pregenerated token string.

```
mapkit.init({
    authorizationCallback: function(done) {
        done("your-token-string");
    },
    language: "es"
});
```

An instance of mapkit emits a `configuration-change` event after MapKit JS initializes, and an `error` event when initialization fails. You can learn more about both of these events in Handling initialization events.

## See Also

### Initialization

Handling initialization events

Respond to events that trigger when MapKit JS initializes.

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

