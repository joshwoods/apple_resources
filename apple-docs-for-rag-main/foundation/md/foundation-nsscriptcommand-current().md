

- Foundation
- NSScriptCommand
-  current() 

Type Method

# current()

If a command is being executed in the current thread by Cocoa scripting’s built-in Apple event handling, return the command.

Mac Catalyst 13.0+macOS 10.0+

``` source
class func current() -> NSScriptCommand?
```

## Discussion

A command is being executed in the current thread by Cocoa scripting’s built-in Apple event handling if an instance of `NSScriptCommand` is handling an execute() message at this instant as the result of the dispatch of an Apple event. Returns `nil` otherwise. scriptErrorNumber and scriptErrorString messages sent to the returned command object will affect the reply event sent to the sender of the event from which the command was constructed, if the sender has requested a reply.

A suspended command is not considered the current command. If a command is suspended and no other command is being executed in the current thread, current() returns `nil`.

