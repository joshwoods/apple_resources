

- WebKit
- WKUserScript
-  init(source:injectionTime:forMainFrameOnly:in:) 

Initializer

# init(source:injectionTime:forMainFrameOnly:in:)

Creates a user script object that is scoped to a particular content world.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
init(
    source: String,
    injectionTime: WKUserScriptInjectionTime,
    forMainFrameOnly: Bool,
    in contentWorld: WKContentWorld
)
```

## Parameters 

`source`  

The script’s source code.

`injectionTime`  

The time at which to inject the script into the webpage. For a list of possible values, see WKUserScriptInjectionTime.

`forMainFrameOnly`  

A Boolean value that indicates whether to inject the script into the main frame. Specify true to inject the script only into the main frame, or false to inject it into all frames.

`contentWorld`  

The namespace in which to evaluate the script. This parameter doesn’t apply to changes your script makes to the underlying web content, such as the document’s DOM structure. Those changes remain visible to all scripts, regardless of which content world you specify. For more information about content worlds, see WKContentWorld.

## Return Value

An initialized user script, or `nil` if initialization failed.

## See Also

### Creating a User Script Object

init(source: String, injectionTime: WKUserScriptInjectionTime, forMainFrameOnly: Bool)

Creates a user script object that contains the specified source code and attributes.

