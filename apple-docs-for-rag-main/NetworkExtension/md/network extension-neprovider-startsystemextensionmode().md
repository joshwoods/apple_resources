

- Network Extension
- NEProvider
-  startSystemExtensionMode() 

Type Method

# startSystemExtensionMode()

Starts the Network Extension machinery from inside a System Extension.

macOS 10.15+

``` source
class func startSystemExtensionMode()
```

## Discussion

Call this method as early as possible after your system extension starts.

Once called, this class method causes your system extension to start handling requests from the Network Extension session manager daemon to instantiate appropriate NEProvider subclass instances. The system extension must declare a mapping of Network Extension extension points to NEProvider subclass instances in its `Info.plist`. The following example shows this mapping:

```
NetworkExtension
    NEProviderClasses

        com.apple.networkextension.app-proxy
        $(PRODUCT_MODULE_NAME).AppProxyProvider
        com.apple.networkextension.filter-data
        $(PRODUCT_MODULE_NAME).FilterDataProvider

```

