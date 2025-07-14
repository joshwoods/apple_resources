

- Core Services
- Apple Events
-  Keyword Attribute Constants 

# Keyword Attribute Constants

Specify keyword values for Apple event attributes.

## Overview

These constants are keyword constants for Apple event attributes. An Apple event consists of attributes (which identify the Apple event and denote its task) and, often, parameters (which contain information to be used by the target application). An Apple event attribute is a descriptor that identifies the event class, event ID, target application, or some other characteristic of the Apple event. Taken together, the attributes of an Apple event denote the task to be performed on any data specified in the Apple event’s parameters.

Keywords are arbitrary names used by the Apple Event Manager to keep track of various descriptors. Your application cannot examine the contents of an Apple event directly. Instead, you call Apple Event Manager routines such as those described in Getting Data or Descriptors From Apple Events and Apple Event Records to request attributes and parameters by keyword.

See also Keyword Parameter Constants.

### Version-Notes

The constant `keyReplyRequestedAttr` was added in OS X version 10.3.

## Topics

### Constants

var keyTransactionIDAttr: AEKeyword

Transaction ID identifying a series of Apple events that are part of one transaction.

var keyReturnIDAttr: AEKeyword

Return ID for a reply Apple event.

var keyEventClassAttr: AEKeyword

Event class of an Apple event. See AEAddressDesc.

var keyEventIDAttr: AEKeyword

Event ID of an Apple event. See AEAddressDesc.

var keyAddressAttr: AEKeyword

Address of a target or client application. See also AEAddressDesc.

var keyOptionalKeywordAttr: AEKeyword

List of keywords for parameters of an Apple event that should be treated as optional by the target application.

var keyTimeoutAttr: AEKeyword

Length of time, in ticks, that the client will wait for a reply or a result from the server.

var keyInteractLevelAttr: AEKeyword

Settings for when to allow the Apple Event Manager to bring a server application to the foreground, if necessary, to interact with the user. See AEAddressDesc. (Read-only.)

var keyEventSourceAttr: AEKeyword

Nature of the source application. (Read-only.)

var keyMissedKeywordAttr: AEKeyword

var keyOriginalAddressAttr: AEKeyword

Address of original source of Apple event if the event has been forwarded (available only in version 1.01 or later versions of the Apple Event Manager). See also AEAddressDesc.

var keyReplyRequestedAttr: AEKeyword

A Boolean value indicating whether the Apple event expects to be replied to.

var keyAcceptTimeoutAttr: AEKeyword

var keyActualSenderAuditToken: AEKeyword

var keySenderApplescriptEntitlementsAttr: AEKeyword

var keySenderApplicationIdentifierEntitlementAttr: AEKeyword

var keySenderApplicationSandboxed: AEKeyword

var keySenderAuditTokenAttr: AEKeyword

var keySenderEGIDAttr: AEKeyword

var keySenderEUIDAttr: AEKeyword

var keySenderGIDAttr: AEKeyword

var keySenderPIDAttr: AEKeyword

var keySenderUIDAttr: AEKeyword

