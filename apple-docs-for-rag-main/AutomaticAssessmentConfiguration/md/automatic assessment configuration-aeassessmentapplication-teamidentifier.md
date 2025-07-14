

- Automatic Assessment Configuration
- AEAssessmentApplication
-  teamIdentifier 

Instance Property

# teamIdentifier

The team identifier of the app.

Mac Catalyst 15.0+macOS 12.0+

``` source
var teamIdentifier: String? { get }
```

## Discussion

You can get the team identifier for an app using the `codesign` command line utility:

```
% codesign -v -d /Applications/MyApp.app
```

## See Also

### Creating an assessment application

init(bundleIdentifier: String, teamIdentifier: String?)

Creates a representation of an app using its bundle and team identifiers.

init(bundleIdentifier: String)

Creates a representation of an app using its bundle identifier.

var bundleIdentifier: String

The bundle identifier of the app.

