

- Core Spotlight
- CSSearchableIndex
-  init(name:) 

Initializer

# init(name:)

Returns an on-device index with the specified name.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
init(name: String)
```

## Parameters 

`name`  

A name that pertains to your custom organization.

## Return Value

An on-device index.

## Discussion

If you want to use batching or you want to index items in a specific protection class, you need to use your own index (you can’t perform batch updates on the default index).

## See Also

### Creating an index

class func `default`() -> Self

Returns the default on-device index.

init(name: String, protectionClass: FileProtectionType?)

Returns an on-device index with the specified name and data protection class.

