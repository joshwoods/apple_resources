

- Security Interface
- SFCertificatePanel
-  shared() 

Type Method

# shared()

Returns a fully initialized, singleton certificate panel object.

macOS 10.3+

``` source
@MainActor
class func shared() -> SFCertificatePanel!
```

## Discussion

Use this method if your application displays a single certificate panel or sheet at a time. If your application can display multiple certificate panels or sheets at once, you must allocate separate object instances (using the alloc class method inherited from NSObject) and initialize them (using the init() instance method, also inherited from NSObject) instead of using this class method.

