

- Security
-  errSecCSStaticCodeNotFound 

Global Variable

# errSecCSStaticCodeNotFound

Cannot find code object on disk.

Mac Catalyst 13.0+macOS 10.0+

``` source
var errSecCSStaticCodeNotFound: OSStatus { get }
```

## Discussion

You can get this error if you specify a location on disk and the system can’t find the code at that location or if the system is checking the validity of running code and it can’t find the code on disk that was the source for the code in memory.

