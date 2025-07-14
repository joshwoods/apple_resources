

- InputMethodKit
-  IMKStateSetting 

Protocol

# IMKStateSetting

The `IMKStateSetting` protocol defines methods for setting or accessing values that indicate the state of an input method.

macOS 10.5+

``` source
protocol IMKStateSetting
```

## Topics

### Activating and Deactivating the Server

func activateServer(Any!)

Activates the input method server.

**Required**

func deactivateServer(Any!)

Deactivates the input method server.

**Required**

### Showing a Preferences Window

func showPreferences(Any!)

Displays a preferences window.

**Required**

### Getting the Supported Events

func recognizedEvents(Any!) -> Int

Returns an unsigned integer that contains a union of event masks

**Required**

### Getting the Mode Dictionary

func modes(Any!) -> [AnyHashable : Any]!

Returns the modes dictionary associated with the input method.

**Required**

### Getting and Setting Values

func value(forTag: Int, client: Any!) -> Any!

Returns a value object whose key is the provided tag.

**Required**

func setValue(Any!, forTag: Int, client: Any!)

Set the value for the provided key.

**Required**

## Relationships

### Conforming Types

- IMKInputController

## See Also

### Protocols

protocol IMKMouseHandling

The `IMKMouseHandling` protocol defines methods that your input method can implement to handle mouse events.

IMKServerInput

`IMKServerInput` is an informal protocol that defines methods for receiving text events. This is intentionally not a formal protocol because there are three ways to receive events. An input method chooses one of the following approaches and implements the appropriate methods:

