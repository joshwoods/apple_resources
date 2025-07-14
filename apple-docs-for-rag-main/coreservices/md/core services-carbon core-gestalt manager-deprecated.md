

- Core Services
- Carbon Core
-  Gestalt Manager Deprecated

API Collection

# Gestalt Manager

Investigate the operating environment of your app.

Deprecated

In macOS 10.8 and later, use ProcessInfo or `sysctl` instead.

## Topics

### Result Codes

The most common result codes returned by the Gestalt Manager are listed below.

var gestaltUnknownErr: Int

Specifies an unknown error.

var gestaltUndefSelectorErr: Int

Specifies an undefined selector was passed to the Gestalt Manager.

var gestaltDupSelectorErr: Int

Specifies you tried to add an entry that already existed.

var gestaltLocationErr: Int

Specifies the gestalt function ptr was not in the system heap.

## See Also

### Managers

Component Manager

Find and use components in your app or add custom components to system-provided services, such as QuickTime and Core Audio.

Text Encoding Conversion Manager

Handle text encoding conversion between apps and transfer text across different platforms.

