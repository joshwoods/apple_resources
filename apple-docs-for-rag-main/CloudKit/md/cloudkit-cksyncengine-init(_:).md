

- CloudKit
- CKSyncEngine
-  init(\_:) 

Initializer

# init(\_:)

Creates a sync engine with the specified configuration.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
init(_ configuration: CKSyncEngine.Configuration)
```

## Parameters 

`configuration`  

The attributes of the new sync engine, such as the associated database and the object to use as the engine’s delegate. For more information, see CKSyncEngine.Configuration.

## See Also

### Creating a sync engine

struct Configuration

A type that configures the attributes and behavior of a sync engine.

