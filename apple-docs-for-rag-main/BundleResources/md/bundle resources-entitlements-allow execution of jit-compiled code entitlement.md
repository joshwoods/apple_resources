

- Bundle Resources
- Entitlements
-  Allow execution of JIT-compiled code entitlement 

Property List Key

# Allow execution of JIT-compiled code entitlement

A Boolean value that indicates whether the app may create writable and executable memory using the `MAP_JIT` flag.

macOS 10.7+

## Details 

Key  
com.apple.security.cs.allow-jit

Type  

boolean

## Discussion

You can create memory that’s both writable and executable by passing the `MAP_JIT` flag to the `mmap()` system function. The Hardened Runtime disallows this by default, because it creates a security risk. However, some apps and system frameworks rely on this functionality, typically for performance reasons. Examples include:

- The fast-path of the JavaScriptCore framework

- Certain Python frameworks

- Perl-compatible regular expressions (PCRE)

- An app that creates a dynamically-compiled, proprietary macro language

Without the `Allow execution of JIT-compiled code entitlement`, frameworks that rely on just-in-time (JIT) compilation may fall back to an interpreter. Other code using JIT compilation may crash or behave in unexpected ways.

Digital rights management (DRM) solutions that currently use unsigned executable memory should instead change to using the `MAP_JIT` flag and the entitlement.

To add the entitlement to your app, first enable the Hardened Runtime capability in Xcode, and then under Runtime Exceptions, select Allow Execution of JIT-compiled Code.

## See Also

### Security

App Sandbox

Restrict access to system resources and user data in macOS apps to contain damage if an app becomes compromised.

App Sandbox Entitlement

A Boolean value that indicates whether the app may use access control technology to contain damage to the system and user data if an app is compromised.

**Key:** com.apple.security.app-sandbox

com.apple.security.network.server

A Boolean value indicating whether your app may listen for incoming network connections.

com.apple.security.network.client

A Boolean value indicating whether your app may open outgoing network connections.

Camera entitlement

A Boolean value that indicates whether the app may interact with the built-in and external cameras, and capture movies and still images.

**Key:** com.apple.security.device.camera

com.apple.security.device.microphone

A Boolean value that indicates whether the app may use the microphone.

com.apple.security.device.usb

A Boolean value indicating whether your app may interact with USB devices.

com.apple.security.print

A Boolean value indicating whether your app may print a document.

com.apple.security.device.bluetooth

A Boolean value indicating whether your app may interact with Bluetooth devices.

Address book entitlement

A Boolean value that indicates whether the app may have read-write access to contacts in the user’s address book.

**Key:** com.apple.security.personal-information.addressbook

Location entitlement

A Boolean value that indicates whether the app may access location information from Location Services.

**Key:** com.apple.security.personal-information.location

Calendars entitlement

A Boolean value that indicates whether the app may have read-write access to the user’s calendar.

**Key:** com.apple.security.personal-information.calendars

com.apple.security.files.user-selected.read-only

A Boolean value that indicates whether the app may have read-only access to files the user has selected using an Open or Save dialog.

com.apple.security.files.user-selected.read-write

A Boolean value that indicates whether the app may have read-write access to files the user has selected using an Open or Save dialog.

com.apple.security.files.downloads.read-only

A Boolean value that indicates whether the app may have read-only access to the Downloads folder.

