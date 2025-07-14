

- Core Services
- Launch Services
- 
  - Launch Services
- Deprecated Symbols
- LSLaunchFSRefSpec
-  appRef Deprecated

Instance Property

# appRef

A pointer to a file-system reference designatingthe application to launch; see the *File Manager Reference* inthe Carbon File Management Documentation for a description of the `FSRef` datatype. Set this field to `NULL` torequest that each item in the `itemRefs` arraybe opened in its own preferred application.

macOS 10.0–10.10Deprecated

``` source
var appRef: UnsafePointer!
```

