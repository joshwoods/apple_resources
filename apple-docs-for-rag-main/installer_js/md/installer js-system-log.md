

- Installer JS
- System
-  log 

# log

Generates an Installer log entry with the `JS:` prefix.

``` source
log(logString)
```

## Parameters 

`logString`  

Log-entry text.

## Overview

For some objects, this function may print data that is unavailable or formatted differently when accessed in JavaScript code. To ensure that only data accessible in JavaScript code is shown in the log entry, invoke this function as shown in Listing 1:

system.log(foo + &#39; &#39;)

Listing 1 Logging JavaScript expressions

Such invocation forces the JavaScript interpreter to evaluate the expression and pass a String object to the function.

