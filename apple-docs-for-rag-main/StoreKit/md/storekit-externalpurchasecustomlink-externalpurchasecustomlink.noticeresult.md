

- StoreKit
- ExternalPurchaseCustomLink
-  ExternalPurchaseCustomLink.NoticeResult 

Enumeration

# ExternalPurchaseCustomLink.NoticeResult

The result of showing the disclosure notice.

iOS 18.1+iPadOS 18.1+macOS 15.1+tvOS 18.1+visionOS 2.1+watchOS 11.1+

``` source
enum NoticeResult
```

## Overview

This value is the result of calling showNotice(type:).

If the value is ExternalPurchaseCustomLink.NoticeResult.continued, the customer choses to continue and your app can offer custom links for external purchases. Otherwise, don’t continue.

## Topics

### Getting notice results

case cancelled

The customer chooses to cancel; don’t offer external purchases.

case continued

The customer chooses to continue; the app can offer external purchases.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Displaying the disclosure sheet

static func showNotice(type: ExternalPurchaseCustomLink.NoticeType) async throws -> ExternalPurchaseCustomLink.NoticeResult

Displays the system disclosure notice sheet and asks the customer whether to continue.

enum NoticeType

The custom link out style that informs the type of disclosure notice to display.

