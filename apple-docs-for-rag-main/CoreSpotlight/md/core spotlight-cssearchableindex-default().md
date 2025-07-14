

- Core Spotlight
- CSSearchableIndex
-  default() 

Type Method

# default()

Returns the default on-device index.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class func `default`() -> Self
```

## Return Value

The default on-device index.

## Mentioned in 

Adding your app’s content to Spotlight indexes

## Discussion

If you want to use batching or you want to index items in a specific protection class, you need to use your own index (you can’t perform batch updates on the default index).

## See Also

### Creating an index

init(name: String)

Returns an on-device index with the specified name.

init(name: String, protectionClass: FileProtectionType?)

Returns an on-device index with the specified name and data protection class.

