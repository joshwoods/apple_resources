

- Shared With You
-  SWHighlightCenter 

Class

# SWHighlightCenter

An object that contains a priority-ordered list of universal links to share with the current user.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class SWHighlightCenter
```

## Mentioned in 

Adding custom collaboration to your app

Making your app content shareable

Adding shared content collaboration to your app

## Overview

The system determines which links it surfaces. The app is responsible for updating its UI to reflect the latest highlights list that the system provides.

## Topics

### Setting the delegate

var delegate: (any SWHighlightCenterDelegate)?

The delegate object for the highlight center.

protocol SWHighlightCenterDelegate

The protocol you use to notify the delegate when the list or rank order of surfaced highlights changes.

### Accessing highlights

var highlights: [SWHighlight]

An array of shared highlights.

class var highlightCollectionTitle: String

A localized title to display with a collection of highlights.

### Retrieving collaboration highlights

class var isSystemCollaborationSupportAvailable: Bool

A Boolean value that represents full support for Messages collaboration features.

func collaborationHighlight(forIdentifier: SWCollaborationIdentifier) throws -> SWCollaborationHighlight

Returns a collaboration highlight for a specified collaboration identifier.

func collaborationHighlight(forIdentifier: String) throws -> SWCollaborationHighlight

Returns a collaboration highlight for a specified identifier string.

func getCollaborationHighlight(for: URL, completionHandler: (SWCollaborationHighlight?, (any Error)?) -> Void)

Returns a collaboration highlight for a specified URL.

func getHighlightFor(URL, completionHandler: (SWHighlight?, (any Error)?) -> Void)

Returns a highlight for a specified URL.

func getSignedIdentityProof(for: SWCollaborationHighlight, using: Data, completionHandler: (SWPerson.SignedIdentityProof?, (any Error)?) -> Void)

Signs passed-in data with the local device’s private key.

### Posting highlight events

func postNotice(for: any SWHighlightEvent)

Posts a specified event to the highlight center for display.

func clearNotices(for: SWCollaborationHighlight)

Clears the notices for a specified collaboration highlight.

### Handling errors

enum SWHighlightCenterErrorCode

The error codes for the highlight center.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Highlights

class SWHighlight

An object that represents a universal link to share by any number of contacts in one or more conversations.

