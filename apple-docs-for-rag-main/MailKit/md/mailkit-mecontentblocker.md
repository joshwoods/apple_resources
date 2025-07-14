

- MailKit
-  MEContentBlocker 

Protocol

# MEContentBlocker

An object that provides a set of rules to block content when displaying a message.

macOS 12.0+

``` source
protocol MEContentBlocker : NSObjectProtocol
```

## Overview

A mail content blocker is similar to content blockers for Safari. Mail uses content blockers when it displays message content in a user’s mailbox. If your extension’s `Info.plist` file contains `MEContentBlocker` in the list of MEExtensionCapabilities, MailKit invokes handlerForContentBlocker() to get the object that provides content-blocking rules. The handler returns the content-blocking rules as JSON data from the contentRulesJSON() method.

For more information about content blockers, see Creating a content blocker.

Note

MailKit always applies content-blocking rules for enabled extensions. This is true even if the user clicks the “Load remote content” button on the banner that Mail displays when remote content isn’t loaded.

To indicate that your extension contains a content blocker, add `MEContentBlocker` to the `MEExtensionCapabilities` array in the extension’s `Info.plist` file:

```
NSExtensionAttributes

    MEExtensionCapabilities

        MEContentBlocker

```

## Topics

### Defining Rules to Block Content

func contentRulesJSON() -> Data

The rules, as JSON data, that the system applies when it displays a message.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

