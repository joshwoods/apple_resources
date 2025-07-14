

- Audio Toolbox
-  CAShowFile(\_:\_:) 

Function

# CAShowFile(\_:\_:)

Prints the internal state of an object to a file.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
func CAShowFile(
    _ inObject: UnsafeMutableRawPointer,
    _ inFile: UnsafeMutablePointer
)
```

## Parameters 

`inObject`  

The Core Audio object whose internal state you want to print.

`inFile`  

The file you want to print object state information to

## Discussion

## See Also

### Audio Toolbox Debugging Functions

func CAShow(UnsafeMutableRawPointer)

Prints the internal state of an object to `stdio`.

