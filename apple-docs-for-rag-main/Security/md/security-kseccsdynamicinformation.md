

- Security
-  kSecCSDynamicInformation 

Global Variable

# kSecCSDynamicInformation

Dynamic validity information about running code.

Mac Catalyst 13.0+macOS 10.0+

``` source
var kSecCSDynamicInformation: UInt32 { get }
```

## Discussion

This information cannot be returned for code on disk (represented by a SecStaticCode object).

