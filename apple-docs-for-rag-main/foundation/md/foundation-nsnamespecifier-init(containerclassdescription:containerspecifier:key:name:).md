

- Foundation
- NSNameSpecifier
-  init(containerClassDescription:containerSpecifier:key:name:) 

Initializer

# init(containerClassDescription:containerSpecifier:key:name:)

Invokes the super class’s init(containerClassDescription:containerSpecifier:key:) method and then sets the name instance variable to `name`.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    containerClassDescription classDesc: NSScriptClassDescription,
    containerSpecifier container: NSScriptObjectSpecifier?,
    key property: String,
    name: String
)
```

## See Also

### Related Documentation

Cocoa Scripting Guide

