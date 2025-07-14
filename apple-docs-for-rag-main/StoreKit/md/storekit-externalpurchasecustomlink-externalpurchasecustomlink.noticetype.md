

- StoreKit
- ExternalPurchaseCustomLink
-  ExternalPurchaseCustomLink.NoticeType 

Enumeration

# ExternalPurchaseCustomLink.NoticeType

The custom link out style that informs the type of disclosure notice to display.

iOS 18.1+iPadOS 18.1+macOS 15.1+tvOS 18.1+visionOS 2.1+watchOS 11.1+

``` source
enum NoticeType
```

## Overview

Provide a notice type value when you call showNotice(type:).

## Topics

### Getting notice types

case browser

A notice type that indicates you display external purchases in a destination outside of the app, which can be an alternative marketplace, another app, or a website.

case withinApp

A notice type that indicates that you display the destination in a web view within the app.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Displaying the disclosure sheet

static func showNotice(type: ExternalPurchaseCustomLink.NoticeType) async throws -> ExternalPurchaseCustomLink.NoticeResult

Displays the system disclosure notice sheet and asks the customer whether to continue.

enum NoticeResult

The result of showing the disclosure notice.

