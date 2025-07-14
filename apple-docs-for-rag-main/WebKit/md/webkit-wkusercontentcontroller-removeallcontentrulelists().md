

- WebKit
- WKUserContentController
-  removeAllContentRuleLists() 

Instance Method

# removeAllContentRuleLists()

Removes all rules lists from the content controller.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
func removeAllContentRuleLists()
```

## Discussion

This method removes the rule lists only from the user content controller object. You can still access rule lists from the WKContentRuleListStore objects you used to create them.

## See Also

### Adding and Removing Content Rules

func add(WKContentRuleList)

Adds the specified content rule list to the content controller object.

func remove(WKContentRuleList)

Removes the specified rule list from the content controller object.

class WKContentRuleList

A compiled list of rules to apply to web content.

