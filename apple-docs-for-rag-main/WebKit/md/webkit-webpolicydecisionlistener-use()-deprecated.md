

- WebKit
- WebPolicyDecisionListener
-  use() Deprecated

Instance Method

# use()

Tells the listener to use the resource.

macOS 10.3–10.14Deprecated

``` source
func use()
```

**Required**

## Discussion

If there are pending policy decisions, the next policy delegate method has the opportunity to decide what to do with the resource. This will be either the next navigation policy delegate (if there is a redirect), or the content policy delegate. If there are no pending policy decisions, the resource will be displayed if possible. If there is no document view available to display the resource, then the webView:unableToImplementPolicyWithError:frame: message will be sent to the web view policy delegate with an appropriate error. Invoking this method creates any new windows needed to handle the resource.

## See Also

### Related Documentation

class func registerClass(AnyClass!, representationClass: AnyClass!, forMIMEType: String!)

Specifies the view and representation objects to be used for specific MIME types.

Deprecated

### Making Resource-Usage Decisions

func download()

Tells the listener to download the resource instead of displaying it.

**Required**

Deprecated

func ignore()

Tells the listener to ignore the resource.

**Required**

Deprecated

