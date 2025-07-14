

- Security
-  kSecCSContentInformation 

Global Variable

# kSecCSContentInformation

More information about the file system contents making up the signed code on disk.

Mac Catalyst 13.0+macOS 10.0+

``` source
var kSecCSContentInformation: UInt32 { get }
```

## Discussion

It is not generally advisable to make use of this information, but some utilities (such as software-update tools) may find it useful.

