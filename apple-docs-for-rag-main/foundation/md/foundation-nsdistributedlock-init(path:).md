

- Foundation
- NSDistributedLock
-  init(path:) 

Initializer

# init(path:)

Initializes an `NSDistributedLock` object to use as the lock the file-system entry specified by a given path.

Mac Catalyst 13.0+macOS 10.0+

``` source
init?(path: String)
```

## Parameters 

`path`  

All of `path` up to the last component itself must exist. You can use FileManager to create (and set permissions) for any nonexistent intermediate directories.

## Return Value

An `NSDistributedLock` object initialized to use as the locking object the file-system entry specified by `path`.

## Discussion

For applications to use the lock, `path` must be accessible to—and writable by—all hosts on which the applications might be running.

