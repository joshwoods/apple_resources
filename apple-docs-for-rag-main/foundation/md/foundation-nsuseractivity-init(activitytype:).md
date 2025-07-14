

- Foundation
- NSUserActivity
-  init(activityType:) 

Initializer

# init(activityType:)

Creates a user activity object with the specified type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(activityType: String)
```

## Parameters 

`activityType`  

The type of the activity. The value is a developer-defined string in reverse-DNS format by convention, for example, `com.myCompany.myEditor.editing`.

## Return Value

An NSUserActivity object.

## See Also

### Related Documentation

Handoff Programming Guide

### Creating a user activity object

Creating a user activity object

Identify key user interactions and include the information to restore them later.

convenience init()

Creates a user activity object using the first activity type declared in the app’s information property list file.

Deprecated

