

- WebKit
- WKContentRuleListStore
-  default() 

Type Method

# default()

Returns the default content rule list store.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
class func `default`() -> Self!
```

## Return Value

The default rule list store.

## Discussion

The default store contains the rules that your app created specifically for the current user.

## See Also

### Creating a Content Rule List Store

convenience init!(url: URL!)

Creates a new content rule list store in the specified directory.

