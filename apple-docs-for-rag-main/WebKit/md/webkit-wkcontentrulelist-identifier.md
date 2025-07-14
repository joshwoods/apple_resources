

- WebKit
- WKContentRuleList
-  identifier 

Instance Property

# identifier

The identifier for the rule list.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
var identifier: String! { get }
```

## Discussion

You specify the identifier for your rule lists at compile time in the compileContentRuleList(forIdentifier:encodedContentRuleList:completionHandler:) method of WKContentRuleListStore. You also use this identifier to look up the rules list later.

