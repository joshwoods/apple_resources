

- Foundation
-  NSKeyedArchiveRootObjectKey 

Global Variable

# NSKeyedArchiveRootObjectKey

Archives created using the class method archivedData(withRootObject:) use this key for the root object in the hierarchy of encoded objects. The NSKeyedUnarchiver class method unarchiveObject(with:) looks for this root key as well.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSKeyedArchiveRootObjectKey: String
```

