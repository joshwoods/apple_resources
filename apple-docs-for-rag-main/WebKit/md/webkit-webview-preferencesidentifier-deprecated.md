

- WebKit
- WebView
-  preferencesIdentifier Deprecated

Instance Property

# preferencesIdentifier

The identifier of the receiver’s preferences.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var preferencesIdentifier: String! { get set }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

It is fixed to the keys used to store the receiver’s preferences in the user defaults database. `WebView` objects can share instances of the `WebPreferences` class by using the same preferences identifier.

## See Also

### Related Documentation

var autosaves: Bool

A Boolean that indicates whether or not the receiver’s attributes are automatically stored in the user defaults database.

Deprecated

### Getting and Setting Preferences

var preferences: WebPreferences!

The receiver’s preferences.

Deprecated

