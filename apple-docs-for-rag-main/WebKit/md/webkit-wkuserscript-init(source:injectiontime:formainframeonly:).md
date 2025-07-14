

- WebKit
- WKUserScript
-  init(source:injectionTime:forMainFrameOnly:) 

Initializer

# init(source:injectionTime:forMainFrameOnly:)

Creates a user script object that contains the specified source code and attributes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
init(
    source: String,
    injectionTime: WKUserScriptInjectionTime,
    forMainFrameOnly: Bool
)
```

## Parameters 

`source`  

The script’s source code.

`injectionTime`  

The time at which to inject the script into the webpage. For a list of possible values, see WKUserScriptInjectionTime.

`forMainFrameOnly`  

A Boolean value that indicates whether to inject the script into the main frame. Specify true to inject the script only into the main frame, or false to inject it into all frames.

## Return Value

An initialized user script, or `nil` if initialization failed.

## Discussion

This method sets the script’s content world to the object in the page property of WKContentWorld.

## See Also

### Creating a User Script Object

init(source: String, injectionTime: WKUserScriptInjectionTime, forMainFrameOnly: Bool, in: WKContentWorld)

Creates a user script object that is scoped to a particular content world.

