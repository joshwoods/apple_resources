

- WebKit
- WKWebExtensionContext
-  command(for:) 

Instance Method

# command(for:)

Retrieves the command associated with the given event without performing it.

macOS 15.4+

``` source
@MainActor
func command(for event: NSEvent) -> WKWebExtension.Command?
```

## Parameters 

`event`  

The event for which to retrieve the corresponding command.

## Return Value

The command associated with the event, or `nil` if there is no such command.

## Discussion

Returns the command that corresponds to the provided event, if such a command exists. This provides a way to programmatically determine what action would occur for a given event, without triggering the command.

