

- Foundation
- NSItemProvider
-  registerGroupActivity(preparationHandler:) 

Instance Method

# registerGroupActivity(preparationHandler:)

Registers a group activity instance asynchronously with the specified options.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOS 1.0+

``` source
@nonobjc
func registerGroupActivity(preparationHandler: @escaping () async throws -> ActivityType) where ActivityType : GroupActivity
```

## Parameters 

`preparationHandler`  

The handler the service invokes when it registers the `GroupActivity`.

## See Also

### Registering group activities

func registerGroupActivity&lt;ActivityType>(ActivityType)

Registers a group activity instance with the specificed options.

