

- Accelerate
-  slarrd\_(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# slarrd\_(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
func slarrd_(
    _ range: UnsafePointer,
    _ order: UnsafePointer,
    _ n: UnsafePointer,
    _ vl: UnsafePointer,
    _ vu: UnsafePointer,
    _ il: UnsafePointer,
    _ iu: UnsafePointer,
    _ gers: UnsafePointer?,
    _ reltol: UnsafePointer,
    _ d: UnsafePointer?,
    _ e: UnsafePointer?,
    _ e2: UnsafePointer?,
    _ pivmin: UnsafePointer,
    _ nsplit: UnsafePointer,
    _ isplit: UnsafePointer?,
    _ m: UnsafeMutablePointer,
    _ w: UnsafeMutablePointer?,
    _ werr: UnsafeMutablePointer?,
    _ wl: UnsafeMutablePointer,
    _ wu: UnsafeMutablePointer,
    _ iblock: UnsafeMutablePointer?,
    _ indexw: UnsafeMutablePointer?,
    _ work: UnsafeMutablePointer,
    _ iwork: UnsafeMutablePointer?,
    _ info: UnsafeMutablePointer
)
```

## See Also

### Functions

func caxpy_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func ccopy_(UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cdotc_(OpaquePointer, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cdotu_(OpaquePointer, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cgbmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cgemm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cgemv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cgerc_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cgeru_(UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func chbmv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func chemm_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func chemv_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cher2_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cher2k_(UnsafePointer&lt;CChar>, UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;__LAPACK_int>, OpaquePointer, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

func cher_(UnsafePointer&lt;CChar>, UnsafePointer&lt;__LAPACK_int>, UnsafePointer&lt;Float>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>, OpaquePointer?, UnsafePointer&lt;__LAPACK_int>)

