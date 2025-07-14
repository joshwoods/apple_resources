

- RealityKit
- ActionHandlerProtocol
-  register(\_:) 

Type Method

# register(\_:)

Registers a handler that responds to raised action events for a particular action type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func register(_ creationHandler: @escaping (Self.EventType) -> (any ActionHandlerProtocol)?)
```

**Required** Default implementations provided.

## Parameters 

`creationHandler`  

The closure that instantiates the handler.

## Default Implementations

### ActionHandlerProtocol Implementations

static func register((Self.EventType) -> (any ActionHandlerProtocol)?)

static func register((Self.EventType) -> (any ActionHandlerProtocol)?)

Registers a handler that creates an action handler, and subscribes to one or more events.

