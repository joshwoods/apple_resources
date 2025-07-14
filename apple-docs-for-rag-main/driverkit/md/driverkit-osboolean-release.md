

- DriverKit
- OSBoolean
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

### Configuring a Boolean Type

free

retain

Retains the OSObject instance

OSBooleanPtr

