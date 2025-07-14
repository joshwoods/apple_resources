

- Automatic Assessment Configuration
- AEAssessmentApplication
-  bundleIdentifier 

Instance Property

# bundleIdentifier

The bundle identifier of the app.

iOS 17.5+iPadOS 17.5+Mac Catalyst 15.0+macOS 12.0+

``` source
var bundleIdentifier: String { get }
```

## Discussion

You can get the bundle identifier for an app using the `codesign` command line utility:

```
% codesign -v -d /Applications/MyApp.app
```

## See Also

### Creating an assessment application

init(bundleIdentifier: String, teamIdentifier: String?)

Creates a representation of an app using its bundle and team identifiers.

init(bundleIdentifier: String)

Creates a representation of an app using its bundle identifier.

var teamIdentifier: String?

The team identifier of the app.

