

- App Store Connect API
- Game Center
- Expressions
-  Evaluating a Boolean value 

Article

# Evaluating a Boolean value

Return given values for true and false results of a conditional.

## Overview

Use the `if()` function in the expression of a matchmaking rule to return values depending on a Boolean conditional. For example, `if (true, `0.0`, `1.0`)` returns `0.0`, and `if (false, `0.0`, `1.0`)` returns `1.0`.

### Declaration

```
any if(boolean $condition, any $ifTrue, any $ifFalse)
```

### Parameters

`condition`  
An expression that evaluates to a Boolean value.

`ifTrue`  
The value to return if `condition` is `true`.

`ifFalse`  
The value to return if `condition` is `false`.

### Return value

Returns `ifTrue` if `condition` is `true`; otherwise, `ifFalse`.

