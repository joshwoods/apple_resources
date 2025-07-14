

- SwiftData
- ModelConfiguration
- ModelConfiguration.GroupContainer
-  identifier(\_:) 

Type Method

# identifier(\_:)

Tells SwiftData to use the specified group container as the root location for the app’s persistent storage.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
static func identifier(_ groupName: String) -> ModelConfiguration.GroupContainer
```

## Parameters 

`groupName`  

The identifier of the group container to use. You find these in the App Groups capabilities section of your Xcode project. For more information, see Configuring app groups.

## See Also

### Getting discovery options

static var automatic: ModelConfiguration.GroupContainer

Tells SwiftData to use the app’s primary group container as the root location for the persistent storage.

static var none: ModelConfiguration.GroupContainer

Prevents SwiftData from using a group container as the root location for the app’s persistent storage.

