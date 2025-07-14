

- Core Services
- Apple Events
-  Descriptor Type Constants 

# Descriptor Type Constants

Specify types for descriptors.

## Overview

The constants described here specify the data type for a descriptor and show the kind of data stored in a descriptor with that type.

Descriptors are the building blocks used by the Apple Event Manager to construct Apple event attributes and parameters. A descriptor is a data structure of type AEDesc, which consists of data storage and a descriptor type that identifies the type of the data. A descriptor type is defined by the data type DescType. AppleScript defines descriptor type constants for a wide variety of common data types. For additional types, see Numeric Descriptor Type Constants and Other Descriptor Type Constants. For a complete listing, including data types such as units of length, weight, and volume, see the Apple Event Manager and Open Scripting Architecture header files.

For the constant `typeApplicationURL`, the data that specifies the application URL takes the following format:

eppc://[username[:password]@]host/AppName[[?uid=#]&amp;[pid=#]]

As indicated by this format:

- `username` is optional. If present, an `'@'` must appear before the host name. `password` is optional. If present, `username` is not optional, and the password must be separated from the username by a `':'` and must precede the `'@'`. `AppName` is not optional; if it contains non-UTF-8 characters or white space, it must be URL-encoded (for example, `My%20Application`).

- `uid` and `pid` are optional. If `pid` is present, `uid` and `AppName` are ignored and the event is delivered only to applications with the given process id. If `uid` is present, events are directed to the application name owned by the given user id.

The following are examples of valid URLs:

eppc://Steve%20Zellers:wombat@grrr.apple.com/Microsoft%20Word
eppc://Steve%20Zellers:wombat@grrr.apple.com/Microsoft%20Word?pid=1284

The availability of user identifiers provides enhanced Apple event support for Fast User Switching. Such identifiers make it possible to send Apple events to applications running in any session, if the uids of the processes match. `'root'` (or `uid 0`) processes are allowed to send Apple events to any process in any session. Non-root processes can only target applications that match their uid.

## Topics

### Constants

var typeAEList: DescType

List of descriptors.

var typeAERecord: DescType

List of keyword-specified descriptors.

var typeAppleEvent: DescType

Apple event.

var typeTrue: DescType

`TRUE` Boolean value.

var typeFalse: DescType

`FALSE` Boolean value.

var typeAlias: DescType

Alias.

var typeEnumerated: DescType

Enumerated data.

var typeType: DescType

Four-character code for event class or event ID

var typeAppParameters: DescType

Process Manager launch parameters.

var typeProperty: DescType

Apple event object property.

var typeFSRef: DescType

File system reference. Use in preference to file system specifications (`typeFSS`).

var typeFileURL: DescType

A file URL. That is, the associated data consists of the bytes of a UTF-8 encoded URL with a scheme of "file". This type is appropriate for describing a file that may not yet exist—see Technical Note 2022 for more information.

var typeKeyword: DescType

Apple event keyword.

var typeSectionH: DescType

Handle to a section record. (Deprecated.)

var typeWildCard: DescType

Matches any type.

var typeApplSignature: DescType

Application signature.

var typeProcessSerialNumber: DescType

A process serial number. See also AEAddressDesc.

var typeApplicationURL: DescType

For specifying an application by URL. See Discussion section below for important information.

var typeNull: DescType

A null data storage pointer. When resolving an object specifier, an object with a null storage pointer specifies the default container at the top of the container hierarchy.

var typeBookmarkData: DescType

var typeEventRecord: DescType

var typeFixed: DescType

var typeQDRectangle: DescType

