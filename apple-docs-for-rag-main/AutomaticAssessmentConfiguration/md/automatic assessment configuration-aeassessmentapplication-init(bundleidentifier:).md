

- Automatic Assessment Configuration
- AEAssessmentApplication
-  init(bundleIdentifier:) 

Initializer

# init(bundleIdentifier:)

Creates a representation of an app using its bundle identifier.

iOS 17.5+iPadOS 17.5+Mac Catalyst 15.0+macOS 12.0+

``` source
init(bundleIdentifier: String)
```

## Parameters 

`bundleIdentifier`  

The bundle identifier of the app.

## Discussion

You can get the bundle identifier for an app using the `codesign` command line utility:

```
% codesign -v -d /Applications/MyApp.app
```

However, it’s typically more secure to specify both the bundle and team identifiers when creating an app representation using init(bundleIdentifier:teamIdentifier:).

## See Also

### Creating an assessment application

init(bundleIdentifier: String, teamIdentifier: String?)

Creates a representation of an app using its bundle and team identifiers.

var bundleIdentifier: String

The bundle identifier of the app.

var teamIdentifier: String?

The team identifier of the app.

