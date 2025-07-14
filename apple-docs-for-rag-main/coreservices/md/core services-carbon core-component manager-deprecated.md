

- Core Services
- Carbon Core
-  Component Manager Deprecated

API Collection

# Component Manager

Find and use components in your app or add custom components to system-provided services, such as QuickTime and Core Audio.

Deprecated

The Component Manager is deprecated in macOS 10.8 and later.

If your app defines custom components to extend functionality, you can instead create a custom a plug-in to replicate the functionality you need. For more information, see Code Loading Programming Topics.

If your app loads audio units and audio codecs, use Audio Component Services instead. For more information, see `Audio Component Services`.

## Topics

### Result Codes

The result codes defined by the Component Manager are listed below.

var invalidComponentID: Int

Invalid component ID.

var validInstancesExist: Int

This component has open connections.

var componentNotCaptured: Int

This component has not been captured.

var componentDontRegister: Int

var unresolvedComponentDLLErr: Int

var retryComponentRegistrationErr: Int

var badComponentSelector: Int

Component does not support the specified request code.

var badComponentInstance: Int

Invalid component passed to Component Manager.

## See Also

### Managers

Gestalt Manager

Investigate the operating environment of your app.

Text Encoding Conversion Manager

Handle text encoding conversion between apps and transfer text across different platforms.

