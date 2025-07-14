

- Foundation
- NSBundleResourceRequest
-  init(tags:bundle:) 

Initializer

# init(tags:bundle:)

Initializes a resource request for managing the on-demand resources marked with any of the set of specified tags. The managed resources are loaded into the specified bundle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    tags: Set,
    bundle: Bundle
)
```

## Parameters 

`tags`  

A set of strings, with each string specifying a tag assigned to resources stored in `bundle`. The value must not be `nil`.

`bundle`  

The bundle used to store the loaded resources. Pass `nil` for the main bundle. The bundle must be the same as the one used in the Xcode project for all the resources marked with the specified tags.

## Return Value

The initialized resource request.

## See Also

### Initializing a Resource Request

convenience init(tags: Set&lt;String>)

Initializes a resource request for managing the on-demand resources marked with any of the set of specified tags. The managed resources are loaded into the main bundle.

