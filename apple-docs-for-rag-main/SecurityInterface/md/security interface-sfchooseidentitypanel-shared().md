

- Security Interface
- SFChooseIdentityPanel
-  shared() 

Type Method

# shared()

Returns a fully initialized, singleton choose identity panel object.

macOS 10.3+

``` source
@MainActor
class func shared() -> SFChooseIdentityPanel!
```

## Discussion

Use this method if your application displays a single choose identity panel or sheet at a time. If your application can display multiple choose identity panels or sheets at once, you must allocate separate object instances (using the alloc class method inherited from NSObject) and initialize them (using the init() instance method, also inherited from NSObject) instead of using this class method.

