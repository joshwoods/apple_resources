

- Foundation
- NSItemProvider
-  registerGroupActivity(\_:) 

Instance Method

# registerGroupActivity(\_:)

Registers a group activity instance with the specificed options.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOS 1.0+

``` source
@nonobjc
func registerGroupActivity(_ activity: ActivityType) where ActivityType : GroupActivity
```

## Parameters 

`activity`  

The `GroupActivity` to register.

## See Also

### Registering group activities

func registerGroupActivity&lt;ActivityType>(preparationHandler: () async throws -> ActivityType)

Registers a group activity instance asynchronously with the specified options.

