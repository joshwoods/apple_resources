

- Automatic Assessment Configuration
- AEAssessmentApplication
-  init(bundleIdentifier:teamIdentifier:) 

Initializer

# init(bundleIdentifier:teamIdentifier:)

Creates a representation of an app using its bundle and team identifiers.

Mac Catalyst 15.0+macOS 12.0+

``` source
init(
    bundleIdentifier: String,
    teamIdentifier: String?
)
```

## Parameters 

`bundleIdentifier`  

The bundle identifier of the app.

`teamIdentifier`  

The team identifier of the team that distributes the app.

## Discussion

You can get the bundle and team identifiers for an app using the `codesign` command line utility:

```
% codesign -v -d /Applications/MyApp.app
```

## See Also

### Creating an assessment application

init(bundleIdentifier: String)

Creates a representation of an app using its bundle identifier.

var bundleIdentifier: String

The bundle identifier of the app.

var teamIdentifier: String?

The team identifier of the app.

