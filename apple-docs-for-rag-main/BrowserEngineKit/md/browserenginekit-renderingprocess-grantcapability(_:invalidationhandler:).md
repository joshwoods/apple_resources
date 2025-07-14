

- BrowserEngineKit
- RenderingProcess
-  grantCapability(\_:invalidationHandler:) 

Instance Method

# grantCapability(\_:invalidationHandler:)

Grants the specified capability to the process, calling the handler when the capability becomes invalid.

iOS 17.6+iPadOS 17.6+

``` source
func grantCapability(
    _ capability: ProcessCapability,
    invalidationHandler: @escaping () -> Void
) throws -> ProcessCapability.Grant
```

## Parameters 

`capability`  

The capability to grant.

`invalidationHandler`  

A closure that the system calls when the capability becomes invalid.

## Return Value

A ProcessCapability.Grant object that represents the granted capability.

## Overview

When the process no longer needs the capability, call invalidate() on the returned object.

## See Also

### Coordinating processes

func grantCapability(ProcessCapability) throws -> ProcessCapability.Grant

Grants the specified capability to the process.

func createVisibilityPropagationInteraction() -> any UIInteraction

Returns an interaction that associates a view with the rendering process.

