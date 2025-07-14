

- Group Activities
- GroupActivity
-  metadata 

Instance Property

# metadata

A description of the activity, and optional image to display to the user.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var metadata: GroupActivityMetadata { get async }
```

**Required**

## Discussion

The system accesses this property when it’s ready to invite other participants to join the activity. Don’t access this property directly. Instead, implement it in your custom activity types and provide descriptive information about the current activity. For example, provide the title of the activity and an image that illustrates the activity.

## See Also

### Specifying the activity details

static var activityIdentifier: String

An app-defined string that uniquely identifies the activity.

**Required** Default implementation provided.

