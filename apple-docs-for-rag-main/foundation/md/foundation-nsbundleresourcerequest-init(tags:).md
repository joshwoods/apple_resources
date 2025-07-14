

- Foundation
- NSBundleResourceRequest
-  init(tags:) 

Initializer

# init(tags:)

Initializes a resource request for managing the on-demand resources marked with any of the set of specified tags. The managed resources are loaded into the main bundle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(tags: Set)
```

## Parameters 

`tags`  

A set of strings, with each string specifying a tag assigned to resources stored in the main bundle. The value must not be `nil`.

## Return Value

The initialized resource request.

## See Also

### Related Documentation

class Bundle

A representation of the code and resources stored in a bundle directory on disk.

On-Demand Resources Guide

### Initializing a Resource Request

init(tags: Set&lt;String>, bundle: Bundle)

Initializes a resource request for managing the on-demand resources marked with any of the set of specified tags. The managed resources are loaded into the specified bundle.

