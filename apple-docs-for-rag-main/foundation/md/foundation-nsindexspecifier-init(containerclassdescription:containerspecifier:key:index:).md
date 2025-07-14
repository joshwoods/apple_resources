

- Foundation
- NSIndexSpecifier
-  init(containerClassDescription:containerSpecifier:key:index:) 

Initializer

# init(containerClassDescription:containerSpecifier:key:index:)

Initializes an allocated NSIndexSpecifier object with a class description, container specifier, collection key, and object index.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    containerClassDescription classDesc: NSScriptClassDescription,
    containerSpecifier container: NSScriptObjectSpecifier?,
    key property: String,
    index: Int
)
```

## Parameters 

`classDesc`  

Description for the container of the collection.

`container`  

Container of the collection.

`property`  

Name of the collection.

`index`  

The object within the `key` collection the index specifier is to identify.

## Return Value

Initialized NSIndexSpecifier object with its `index` property set to `objectIndex`.

## Discussion

Invokes the super class’s init(containerClassDescription:containerSpecifier:key:) method and sets the `index` property of the index specifier to `objectIndex`.

## See Also

### Related Documentation

Cocoa Scripting Guide

