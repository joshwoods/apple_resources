

- CoreAudioKit
- AUCustomViewPersistentData
-  customViewPersistentData 

Instance Property

# customViewPersistentData

Called by the host application to obtain view state data from a custom Cocoa view.

macOS 10.6+

``` source
unowned(unsafe) var customViewPersistentData: NSDictionary? { get set }
```

**Required**

## Return Value

A dictionary containing view state data.

## Discussion

The host application should call this method before closing the view.

