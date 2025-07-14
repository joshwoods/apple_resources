

- Core Services
-  Launch Services 

API Collection

# Launch Services

Launch and open documents in other apps from your current app process.

## Overview

macOS Launch Services is an API that enables a running app to open other apps or their document files, similar to the Finder or the Dock. Using Launch Services, an app can perform such tasks as:

- Open (launch or activate) another app

- Open a document or a URL in another app

- Identify the preferred app for opening a document or URL

- Register information about the kinds of document files and URLs an app can open

- Obtain information for displaying a file or URL on the screen, such as its icon, display name, and kind string

- Maintain and update the contents of the Recent Items menu

Launch Services eliminates apps having to query the Finder to open an app, document, or URL for them. The macOS Finder itself uses Launch Services to perform such tasks. Because the Finder performs no additional processing beyond calling Launch Services, any client using Launch Services for these purposes behaves identically to the Finder.

## Topics

### Locating an App

The functions in this section locate and test the preferred app for opening an item or a family of items, or the app that matches a set of defining characteristics.

func LSCopyDefaultApplicationURLForURL(CFURL, LSRolesMask, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFURL>?

Returns the app that opens an item.

Deprecated

func LSCopyDefaultApplicationURLForContentType(CFString, LSRolesMask, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFURL>?

Returns the app that opens a content type.

Deprecated

func LSCopyApplicationURLsForURL(CFURL, LSRolesMask) -> Unmanaged&lt;CFArray>?

Locates all known apps suitable for opening an item for the specified URL.

Deprecated

func LSCanURLAcceptURL(CFURL, CFURL, LSRolesMask, LSAcceptanceFlags, UnsafeMutablePointer&lt;DarwinBoolean>) -> OSStatus

Tests whether an app can accept (open) an item for a URL.

func LSCopyApplicationURLsForBundleIdentifier(CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFArray>?

Locates all URLs for apps that correspond to the specified bundle identifier.

Deprecated

### Opening Items

The functions in this section open a designated item or a collection of items, or launch or activate a designated app.

func LSOpenCFURLRef(CFURL, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>?) -> OSStatus

Opens an item for a URL in the default manner in its preferred app.

func LSOpenFromURLSpec(UnsafePointer&lt;LSLaunchURLSpec>, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>?) -> OSStatus

Opens one or more items for a URL in the preferred apps or a designated app.

struct LSLaunchURLSpec

The specification for launching an app, opening items, or both, along with related information.

class LSSharedFileList

A persistent list of file-system objects.

class LSSharedFileListItem

A file-system object in the shared file list.

### Registering an App

The functions in this section register an app in the Launch Services database.

func LSRegisterURL(CFURL, Bool) -> OSStatus

Registers an app, using a URL, in the Launch Services database.

### Working with Role Handlers

The functions in this section get and set bundle identifiers for handlers of specified content types and URL schemes.

func LSCopyAllRoleHandlersForContentType(CFString, LSRolesMask) -> Unmanaged&lt;CFArray>?

Locates an array of bundle identifiers for apps capable of handling a specified content type with the specified roles.

Deprecated

func LSCopyDefaultRoleHandlerForContentType(CFString, LSRolesMask) -> Unmanaged&lt;CFString>?

Returns the bundle identifier of the user’s preferred default handler for the specified content type with the specified role.

Deprecated

func LSSetDefaultRoleHandlerForContentType(CFString, LSRolesMask, CFString) -> OSStatus

Sets the user’s preferred default handler for the specified content type in the specified roles.

Deprecated

func LSSetDefaultHandlerForURLScheme(CFString, CFString) -> OSStatus

Sets the user’s preferred default handler for the specified URL scheme.

Deprecated

struct LSRolesMask

The specification that sets the desired role or roles for an app to claim for an item or a family of items.

### Understanding the Quarantine Properties Dictionary

let kLSQuarantineAgentBundleIdentifierKey: CFString

The bundle identifier of the quarantining agent.

let kLSQuarantineAgentNameKey: CFString

The app name of the quarantining agent.

let kLSQuarantineTimeStampKey: CFString

The date and time of the item’s quarantine.

let kLSQuarantineTypeKey: CFString

A symbolic string identifying the reason for the quarantine.

let kLSQuarantineDataURLKey: CFString

The actual URL of the quarantined item.

let kLSQuarantineOriginURLKey: CFString

The URL of the resource originally hosting the quarantined item.

### Identifying the Quarantine Type

let kLSQuarantineTypeCalendarEventAttachment: CFString

The type when the data is an attachment from a calendar event.

let kLSQuarantineTypeEmailAttachment: CFString

The type when the data is an attachment from an email message.

let kLSQuarantineTypeInstantMessageAttachment: CFString

The type when the data is an attachment from a message.

let kLSQuarantineTypeOtherAttachment: CFString

The type when the data is an attachment from a generic source.

let kLSQuarantineTypeOtherDownload: CFString

The type when the data is from a download.

let kLSQuarantineTypeWebDownload: CFString

The type when the data is from a website download.

### Constants

This section describes the constants in the Launch Services API.

struct LSLaunchFlags

The specification for launching an app.

struct LSAcceptanceFlags

The specification that determines whether an app can accept (open) an item.

struct LSItemInfoFlags

The specification that provides information about an item.

struct LSHandlerOptions

The specification that controls the selection of handlers.

struct LSRequestedInfo

The specification that controls which information to obtain about an item.

Unknown Type or Creator

Represents an unknown file type or creator.

### Result Codes

This section lists the most common result codes that Launch Services functions return.

var kLSAppInTrashErr: OSStatus

The app can’t run because it’s inside a Trash folder.

var kLSUnknownErr: OSStatus

An unknown error has occurred.

var kLSNotAnApplicationErr: OSStatus

The item for registration is not an app.

var kLSDataUnavailableErr: OSStatus

Data of the desired type is not available (for example, there is no kind string).

var kLSApplicationNotFoundErr: OSStatus

No app in the Launch Services database matches the input criteria.

var kLSDataErr: OSStatus

Improper data structure.

var kLSLaunchInProgressErr: OSStatus

A launch of the app is already in progress.

var kLSServerCommunicationErr: OSStatus

There is a problem communicating with the server process that maintains the Launch Services database.

var kLSCannotSetInfoErr: OSStatus

The system can’t hide the filename extension.

var kLSIncompatibleSystemVersionErr: OSStatus

The requested app can’t run on the current macOS version.

var kLSNoLaunchPermissionErr: OSStatus

The user doesn’t have permission to launch the app on a managed network.

var kLSNoExecutableErr: OSStatus

The executable file is missing or has an unusable format.

var kLSMultipleSessionsNotSupportedErr: OSStatus

The requested app can’t run simultaneously in two different user sessions.

### Deprecated

Deprecated Symbols

Apple has deprecated these symbols and no longer recommends using them.

