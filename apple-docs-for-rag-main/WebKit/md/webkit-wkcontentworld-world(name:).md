

- WebKit
- WKContentWorld
-  world(name:) 

Type Method

# world(name:)

Returns the custom content world with the specified name.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
class func world(name: String) -> WKContentWorld
```

## Parameters 

`name`  

The name of the content world you want. If no content world with that name exists, this method creates a new WKContentWorld object and returns it. The next time you request a content world with the same name, this method returns the object it previously created.

## Return Value

The content world with the specified name.

## Discussion

Use this method to create unique content worlds for your script code. For example, if you execute scripts from multiple JavaScript extensions, you might use this method to create a content world based on a unique string associated with that extension.

## See Also

### Retrieving a Custom Content World

var name: String?

The name of a custom content world.

