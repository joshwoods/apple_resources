

- Objective-C Runtime
- NSObject
-  candidates(\_:) 

Instance Method

# candidates(\_:)

Returns an array of candidates.

macOS

``` source
func candidates(_ sender: Any!) -> [Any]!
```

## Parameters 

`sender`  

The client object requesting the candidates.

## Return Value

An array of candidates. The returned array should be an autoreleased object.

## Discussion

An input method should look up its currently composed string and return a list of candidate strings that the composed string might map to.

