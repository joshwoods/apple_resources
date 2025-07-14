

- Application Services
- ApplicationServices Structures
- OpenCPicParams
-  srcRect 

Instance Property

# srcRect

The optimal bounding rectangle for the resolution indicated by the `hRes` and `vRes` fields. To display a picture at a resolution other than that specified in the `hRes` and `vRes` fields, your application should compute an appropriate destination rectangle by scaling the image’s width and height by the destination resolution divided by the source resolution.

macOS 10.0+

``` source
var srcRect: Rect
```

