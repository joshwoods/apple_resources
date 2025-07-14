

- WebKit
- WKUserContentController
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the specified rule list from the content controller object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
func remove(_ contentRuleList: WKContentRuleList)
```

## Parameters 

`contentRuleList`  

The rule list to remove.

## Discussion

This method removes the rule list only from the user content controller object. You can still access the rule list from the WKContentRuleListStore object you used to create it.

## See Also

### Adding and Removing Content Rules

func add(WKContentRuleList)

Adds the specified content rule list to the content controller object.

func removeAllContentRuleLists()

Removes all rules lists from the content controller.

class WKContentRuleList

A compiled list of rules to apply to web content.

