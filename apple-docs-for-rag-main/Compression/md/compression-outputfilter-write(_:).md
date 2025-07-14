

- Compression
- OutputFilter
-  write(\_:) 

Instance Method

# write(\_:)

Writes data to the output filter.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func write(_ data: D?) throws where D : DataProtocol
```

## See Also

### Instance Methods

func finalize() throws

Finalizes the stream by flushing all the remaining data in the stream.

