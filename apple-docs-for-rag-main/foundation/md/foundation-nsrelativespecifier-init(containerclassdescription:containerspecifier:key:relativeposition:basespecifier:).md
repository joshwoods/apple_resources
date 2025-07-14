

- Foundation
- NSRelativeSpecifier
-  init(containerClassDescription:containerSpecifier:key:relativePosition:baseSpecifier:) 

Initializer

# init(containerClassDescription:containerSpecifier:key:relativePosition:baseSpecifier:)

Invokes the super class’s init(containerClassDescription:containerSpecifier:key:) method and initializes the relative position and base specifier to `relPos` and `baseSpecifier`.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    containerClassDescription classDesc: NSScriptClassDescription,
    containerSpecifier container: NSScriptObjectSpecifier?,
    key property: String,
    relativePosition relPos: NSRelativeSpecifier.RelativePosition,
    baseSpecifier: NSScriptObjectSpecifier?
)
```

## See Also

### Related Documentation

Cocoa Scripting Guide

