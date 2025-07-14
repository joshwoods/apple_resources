

- Installer JS
- System
-  run 

# run

Launches a given program in the `Resources` directory of the installation package.

``` source
run(programName, args...)
```

## Parameters 

`programName`  

Name of the program to execute.

`args...`  

Arguments passed to the program.

## Return Value

After the program is executed, its exit code. If the program is not executed (see discussion), `undefined`.

## Overview

The `allow-external-scripts` attribute of the `options` element in the distribution definition must be `'yes'` for the program to be launched. And, the Installer application asks the user’s permission before launching the program. See Distribution Definition XML Schema Reference for more information.

## See Also

### Running Programs

runOnce

Launches a given program in the `Resources` directory of the installation package, if it has not been run already.

### Related Documentation

System

An object that provides access to information about the target host.

