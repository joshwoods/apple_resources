

- WebKit
-  WebPolicyDecisionListener Deprecated

Protocol

# WebPolicyDecisionListener

This protocol enables WebView policy delegates to communicate with listener objects. A listener object conforming to this protocol is passed as one of the arguments to web view policy delegate methods.

macOS 10.3–10.14Deprecated

``` source
protocol WebPolicyDecisionListener : NSObjectProtocol
```

## Overview

This protocol allows delegates to handle download decisions asynchronously. For example, the policy delegate may display a sheet, and the listener object gets notified only after the user clicks an OK or Cancel button. You do not directly create objects that conform to this protocol.

## Topics

### Making Resource-Usage Decisions

func download()

Tells the listener to download the resource instead of displaying it.

**Required**

func ignore()

Tells the listener to ignore the resource.

**Required**

func use()

Tells the listener to use the resource.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Related Documentation

WebKit Objective-C Programming Guide

### Setting Policies (Legacy)

protocol WebPolicyDelegateDeprecated

