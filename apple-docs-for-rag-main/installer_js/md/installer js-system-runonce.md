

- Installer JS
- System
-  runOnce 

# runOnce

Launches a given program in the `Resources` directory of the installation package, if it has not been run already.

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

On subsequent invocations with the same arguments, the program is not launched and the exit code of the first execution is returned.

The `allow-external-scripts` attribute of the `options` element in the distribution definition must be `'yes'` for the program to be launched. And, the Installer application asks the user’s permission before launching the program. See Distribution Definition XML Schema Reference for more information.

Use this method instead of run when a program’s exit code using the same arguments is not expected to change.

## See Also

### Running Programs

run

Launches a given program in the `Resources` directory of the installation package.

