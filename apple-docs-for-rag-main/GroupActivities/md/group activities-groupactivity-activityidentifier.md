

- Group Activities
- GroupActivity
-  activityIdentifier 

Type Property

# activityIdentifier

An app-defined string that uniquely identifies the activity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static var activityIdentifier: String { get }
```

**Required** Default implementation provided.

## Mentioned in 

Defining your app’s SharePlay activities

Adding spatial Persona support to an activity

## Discussion

Implement this property and return a value that uniquely identifies the activity within your app. An app may support multiple activities, and each activity requires a unique identifier string. Use reverse-DNS notation for your identifier strings. For example, supply a string like `"com.mycompany.myapp.watchmovie"` for a movie-watching activity.

If you don’t implement this property yourself, the default implementation composes an activity identifier using your app’s bundle identifier and the current class or struct name. For example, if the app’s bundle identifier is `"com.mycompany.myapp"` and your activity type name is `MovieActivity`, the resulting identifier string is `"com.mycompany.myapp.MovieActivity"`.

## Default Implementations

### GroupActivity Implementations

static var activityIdentifier: String

An app-defined string that uniquely identifies the activity.

## See Also

### Specifying the activity details

var metadata: GroupActivityMetadata

A description of the activity, and optional image to display to the user.

**Required**

