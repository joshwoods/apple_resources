

- WebKit
- WebPreferences
-  init(identifier:) Deprecated

Initializer

# init(identifier:)

Returns an initialized `WebPreferences` object, creating one if it does not exist.

macOS 10.3–10.14Deprecated

``` source
init!(identifier anIdentifier: String!)
```

## Parameters 

`anIdentifier`  

A unique identifier for the WebPreferences object

## Return Value

A newly initialized WebPreferences object with the identifier; if an existing `WebPreferences` object with that identifier exists, it is returned instead.

## Discussion

The `anIdentifier` argument should be unique—it is prepended to the keys used to store the receiver’s attributes in the user defaults database. WebView objects can share a WebPreferences object by using the same preferences identifier.

Typically, you do not invoke this method directly. Instead, you set the preferences identifier by sending a preferencesIdentifier message to your WebView object. This method is the designated initializer for the WebPreferences class.

## See Also

### Related Documentation

var identifier: String!

The receiver’s identifier.

Deprecated

