

- Quartz
- IKSaveOptions
-  delegate 

Instance Property

# delegate

Specifies the delegate object.

macOS 10.5+

``` source
unowned(unsafe) var delegate: AnyObject! { get set }
```

## See Also

### Related Documentation

func saveOptions(_ saveOptions: IKSaveOptions!, shouldShowUTType utType: String!) -> Bool

Called to determine if the specified uniform type identifier should be shown in the save panel.

