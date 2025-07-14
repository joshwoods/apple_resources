

- Create ML
- MLDataTable
-  writeCSV(toFile:) 

Instance Method

# writeCSV(toFile:)

Exports a CSV file of the data table to the given directory path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func writeCSV(toFile path: String) throws
```

## Discussion

- path: A file system path where the data table file should be written.

## See Also

### Saving a data table

func write(to: URL) throws

Exports a binary file of the data table to the given directory URL.

func write(toDirectory: String) throws

Exports a binary file of the data table to the given directory path.

func writeCSV(to: URL) throws

Exports a CSV file of the data table to the given directory URL.

