

- Core Services
- Launch Services
-  LSAcceptanceFlags 

Structure

# LSAcceptanceFlags

The specification that determines whether an app can accept (open) an item.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct LSAcceptanceFlags
```

## Overview

These flags are passed to the functions `LSCanRefAcceptItem` and `LSCanURLAcceptURL`.

## Topics

### Creating Acceptance Flags

init(rawValue: OptionBits)

Creates a new acceptance flag from the given raw value.

### Constants

static var acceptDefault: LSAcceptanceFlags

Requests the default behavior that does not require the user interface to log in be presented.

static var acceptAllowLoginUI: LSAcceptanceFlags

Requests that the user interface to log in be presented.

## Relationships

### Conforms To

- OptionSet
- Sendable

