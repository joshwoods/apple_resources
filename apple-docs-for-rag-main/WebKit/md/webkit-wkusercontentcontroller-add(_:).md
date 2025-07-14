

- WebKit
- WKUserContentController
-  add(\_:) 

Instance Method

# add(\_:)

Adds the specified content rule list to the content controller object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
func add(_ contentRuleList: WKContentRuleList)
```

## Parameters 

`contentRuleList`  

The rule list to add. Create and retrieve rules lists using a `WKContentExtensionStore` object.

## Discussion

Call this method to apply a set of content filtering rules to your web view’s configuration.

## See Also

### Adding and Removing Content Rules

func remove(WKContentRuleList)

Removes the specified rule list from the content controller object.

func removeAllContentRuleLists()

Removes all rules lists from the content controller.

class WKContentRuleList

A compiled list of rules to apply to web content.

