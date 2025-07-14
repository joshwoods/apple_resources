

- WebKit
- WKContentRuleListStore
-  init(url:) 

Initializer

# init(url:)

Creates a new content rule list store in the specified directory.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
convenience init!(url: URL!)
```

## Parameters 

`url`  

A URL that specifies a directory. The returned object uses this directory to store its content rules persistently. For example, you might store your app-specific rules in your app’s container directory.

## Return Value

A content rule store associated with the specified directory.

## Discussion

If the specified directory already contains compiled rule lists, this method loads those rules and adds them to the returned object. If you change any rules after creating this object, the store saves those changes to the same directory.

## See Also

### Creating a Content Rule List Store

class func `default`() -> Self!

Returns the default content rule list store.

