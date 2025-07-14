

- BrowserEngineKit
- NetworkingProcess
-  grantCapability(\_:) 

Instance Method

# grantCapability(\_:)

Grants the specified capability to the process.

iOS 17.4+iPadOS 17.4+macOS 14.3+

``` source
func grantCapability(_ capability: ProcessCapability) throws -> ProcessCapability.Grant
```

## Parameters 

`capability`  

The capability to grant.

## Return Value

A ProcessCapability.Grant object that represents the granted capability.

## Overview

When the process no longer needs the capability, call invalidate() on the returned object.

## See Also

### Coordinating processes

func grantCapability(ProcessCapability, invalidationHandler: () -> Void) throws -> ProcessCapability.Grant

Grants the specified capability to the process, calling the handler when the capability becomes invalid.

