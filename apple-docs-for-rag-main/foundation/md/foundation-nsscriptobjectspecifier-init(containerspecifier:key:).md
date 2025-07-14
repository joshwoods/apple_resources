

- Foundation
- NSScriptObjectSpecifier
-  init(containerSpecifier:key:) 

Initializer

# init(containerSpecifier:key:)

Returns an `NSScriptObjectSpecifier` object initialized with a given container specifier and key.

Mac Catalyst 13.0+macOS 10.0+

``` source
convenience init(
    containerSpecifier container: NSScriptObjectSpecifier,
    key property: String
)
```

## Return Value

An `NSScriptObjectSpecifier` object initialized with container specifier `specifier` and key `key`.

## Discussion

The class description of the container is set automatically.

## See Also

### Initializing an object specifier

init(containerClassDescription: NSScriptClassDescription, containerSpecifier: NSScriptObjectSpecifier?, key: String)

Returns an `NSScriptObjectSpecifier` object initialized with the given attributes.

