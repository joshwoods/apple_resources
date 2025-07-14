

- DriverKit
- OSMetaClassBase
-  release 

Instance Method

# release

Releases the OSObject instance

DriverKitiOSiPadOSmacOS

``` source
void release() const;
```

## Discussion

Decreases the retain count of the instance by one. If the count is then zero, frees the object.

## See Also

### Managing the Object Lifecycle

retain

Retains the OSObject instance

