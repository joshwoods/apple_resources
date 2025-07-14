

- WebKit
-  WKContentRuleList 

Class

# WKContentRuleList

A compiled list of rules to apply to web content.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
class WKContentRuleList
```

## Overview

A WKContentRuleList object represents a compiled set of rules for modifying how a webpage loads content. You don’t create a WKContentRuleList directly. Instead, you specify your rules in JSON format and compile them using the compileContentRuleList(forIdentifier:encodedContentRuleList:completionHandler:) method of WKContentRuleListStore. That method compiles your rules into an efficient byte format and returns them in an instance of this class.

Content rule lists use the same syntax as content blocker extensions in Safari. For more information on how to specify the JSON for your rule lists, see Creating a content blocker.

## Topics

### Getting the Rules List Identifier

var identifier: String!

The identifier for the rule list.

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
- Sendable

## See Also

### Adding and Removing Content Rules

func add(WKContentRuleList)

Adds the specified content rule list to the content controller object.

func remove(WKContentRuleList)

Removes the specified rule list from the content controller object.

func removeAllContentRuleLists()

Removes all rules lists from the content controller.

