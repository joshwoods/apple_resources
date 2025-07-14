

- Application Services
- ColorSync Manager
- Profile Access Procedures
-  cmBeginAccess 

Global Variable

# cmBeginAccess

Begin the process of procedural access. This is always the first operation constant passed to the access procedure. If the call is successful, the `cmEndAccess` operation is guaranteed to be the last call to the procedure.

macOS 10.0+

``` source
var cmBeginAccess: Int { get }
```

