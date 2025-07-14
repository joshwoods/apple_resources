

- Create ML
- MLDataTable
-  writeCSV(to:) 

Instance Method

# writeCSV(to:)

Exports a CSV file of the data table to the given directory URL.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func writeCSV(to fileURL: URL) throws
```

## Discussion

- fileURL: The location in the file system to which the data table file should be written.

## See Also

### Saving a data table

func write(to: URL) throws

Exports a binary file of the data table to the given directory URL.

func write(toDirectory: String) throws

Exports a binary file of the data table to the given directory path.

func writeCSV(toFile: String) throws

Exports a CSV file of the data table to the given directory path.

