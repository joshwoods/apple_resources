

- Create ML
- MLDataTable
-  write(to:) 

Instance Method

# write(to:)

Exports a binary file of the data table to the given directory URL.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func write(to directoryURL: URL) throws
```

## Discussion

- directoryURL: The directory location in the file system to which the data table file should be written.

## See Also

### Saving a data table

func write(toDirectory: String) throws

Exports a binary file of the data table to the given directory path.

func writeCSV(to: URL) throws

Exports a CSV file of the data table to the given directory URL.

func writeCSV(toFile: String) throws

Exports a CSV file of the data table to the given directory path.

