# Nephthis-BP-VBO---Extended-Collections-Tools
Additional C# Collection Manipulation actions for use in Blue Prism, heavy reliance on Linq library due to .NET Datatables

## Get Value of Index
Retrieves a value of a specified cell in the table. Indicies start from 0 and count up.

### Inputs:
* Collection - Collection
* Row - Number
* Column - Number

### Outputs:
* Value - Text

## Set Value of Index
Sets a text value of a specifiecd cell in the table. Indicies start from 0 and count up. Assumes cell datatype is String/Text.

### Inputs:
* Collection - Collection
* Row - Number
* Column - Number
* Value - Text

### Outputs:
* Modified Collection - Collection

## Set Value of Index - Collection Type
Sets a text value of a specifiecd cell in the table. Indicies start from 0 and count up. Assumes cell datatype is Collection/DataTable.

### Inputs:
* Collection - Collection
* Row - Number
* Column - Number
* Value - Collection

### Outputs:
* Modified Collection - Collection

## Set Value of Index - Number Type
Sets a text value of a specifiecd cell in the table. Indicies start from 0 and count up. Assumes cell datatype is Number/Double.

### Inputs:
* Collection - Collection
* Row - Number
* Column - Number
* Value - Number

### Outputs:
* Modified Collection - Collection

## Set Value of Index - Date Type
Sets a text value of a specifiecd cell in the table. Indicies start from 0 and count up. Assumes cell datatype is Date/System.DateTime.

### Inputs:
* Collection - Collection
* Row - Number
* Column - Number
* Value - Date

### Outputs:
* Modified Collection - Collection

## Set Value of Index - DateTime Type
Sets a text value of a specifiecd cell in the table. Indicies start from 0 and count up. Assumes cell datatype is DateTime/System.DateTime.

### Inputs:
* Collection - Collection
* Row - Number
* Column - Number
* Value - Datetime

### Outputs:
* Modified Collection - Collection

## Set Value of Index - Flag Type
Sets a text value of a specifiecd cell in the table. Indicies start from 0 and count up. Assumes cell datatype is Flag/Boolean.
### Inputs:
* Collection - Collection
* Row - Number
* Column - Number
* Value - Flag

### Outputs:
* Modified Collection - Collection

## Set Value of Index - Password Type
Sets a text value of a specifiecd cell in the table. Indicies start from 0 and count up. Assumes cell datatype is Password/String.

### Inputs:
* Collection - Collection
* Row - Number
* Column - Number
* Value - Password

### Outputs:
* Modified Collection - Collection

## Set Value of Index - Time Type
Sets a text value of a specifiecd cell in the table. Indicies start from 0 and count up. Assumes cell datatype is Time/System.DateTime.

### Inputs:
* Collection - Collection
* Row - Number
* Column - Number
* Value - Time

### Outputs:
* Modified Collection - Collection

## Set Value of Index - TimeSpan Type
Sets a text value of a specifiecd cell in the table. Indicies start from 0 and count up. Assumes cell datatype is TimeSpan.

### Inputs:
* Collection - Collection
* Row - Number
* Column - Number
* Value - TimeSpan

### Outputs:
* Modified Collection - Collection

## Set Value of Index - Image Type
Sets a text value of a specifiecd cell in the table. Indicies start from 0 and count up. Assumes cell datatype is Image/Drawing.Bitmap.

### Inputs:
* Collection - Collection
* Row - Number
* Column - Number
* Value - Image

### Outputs:
* Modified Collection - Collection

## Set Value of Index - Binary Type
Sets a text value of a specifiecd cell in the table. Indicies start from 0 and count up. Assumes cell datatype is Binary/System.Byte[].

### Inputs:
* Collection - Collection
* Row - Number
* Column - Number
* Value - Binary

### Outputs:
* Modified Collection - Collection

## Find Row Index of Value
Finds the index of a row containing a specified value. The collection MUST have been primed first using the action "Append Autoincriment Column"

### Inputs:
* Collection - Collection
* Value - Text

### Outputs: 
* Row - Number

## Sort Collection
Sorts a collection by a specified column

### Inputs:
* Collection - Collection
* Ascending - Flag
* Column - Text

### Outputs:
* Sorted Collection - Collection

## Search Collection
Returns a collection of filtered results containing rows that match

### Inputs:
* Collection - Collection
* Filter - Text
* Column - Text

### Outputs:
* Sorted Collection - Collection

## Search Collection (cast to string)
Returns a collection of filtered results containing rows that match search, casting the specified column to type Text/String in the process

### Inputs:
* Collection - Collection
* Filter - Text
* Column - Text

### Outputs:
* Sorted Collection - Collection

## Search Collection where value does not start with [x]
Returns a collection of filtered results containing rows that match search, where the value does not start with the specified filter

### Inputs:
* Collection - Collection
* Filter - Text
* Column - Text

### Outputs:
* Sorted Collection - Collection

## Search Collection where value starts with [x]
Returns a collection of filtered results containing rows that match search, where the value starts with the specified filter

### Inputs:
* Collection - Collection
* Filter - Text
* Column - Text

### Outputs:
* Sorted Collection - Collection

## Search Collection where value contains [sql method]
Returns a collection of filtered results containing rows that match search. Used for statements such as: "like %'+char(10)+'%"

### Inputs:
* Collection - Collection
* Filter - Text
* Column - Text

### Outputs:
* Sorted Collection - Collection

## Search Collection where value does not contain [x]
Returns a collection of filtered results containing rows that do not contain the supplied text

### Inputs:
* Collection - Collection
* Filter - Text
* Column - Text

## Sum of Column
Returns a sum of a column

### Inputs:
* Collection - Collection
* Column - Text

### Outputs:
* Sum - Number

## Convert column to Number type
Converts the specified column to type Number/Double

### Inputs:
* Collection - Collection
* Column - Number

### Outputs:
* newData - Collection

## Get Distinct Values
Returns a collection of distinct values for the specified column in a collection

### Inputs:
* Collection - Collection
* Column - Text

### Outputs:
* Sorted Collection - Collection

## Rotate Collection
Converts columns to rows and maintains order. Col 1 = Row 1, Col 2 = Row 2, etc. 1x3 becomes 3x1, 2x7 becomes 7x2, etc.

### Inputs:
* Collection - Collection

### Outputs:
* Rotated Collection - Collection

## Convert column to Text Type
Converts specified column to type Text

### Inputs:
* Collection - Collection
* Column - Number

### Outputs:
* newData - Collection

## Compare Collections by Column
Returns a collection based on Haystack input where column data matches that of Needle input

### Inputs:
* Needle - Collection
* Haystack - Collection
* Column - Text

### Outputs:
* Matching Rows - Collection

## Append Row
Appends one of multiple to a collection using CSV input data

### Inputs:
* Collection - Collection
* CSV Row - Text

### Outputs:
* New Collection - Collection

## Append Autoincriment column
Appends a column of name "AiId" containing a numberic value increasing from 0, representing row indecies

### Inputs:
* Collection - Collection

### Outputs:
* New Collection - Collection

## Append column
Appends a column of a specified BP data type to a collection

### Inputs:
* Collection - Collection
* Name - Text
* Type - Text

### Outputs:
* New Collection - Collection

## Append All
Appends all fields/data from one collection to another

### Inputs:
* Collection A - Collection
* Collection B - Collection

### Outputs:
* Collection Out - Collection

## Delete Row by Index
Deletes a row by specified numberic index, starting with 0

### Inputs:
* Collection - Collection
* Row Index - Number

### Outputs:
* New Collection - Collection

## Delete Empty Rows
WARNING: Only works if all columns are of type Text/String! Ideal for pulling and pruning Excel data

### Inputs:
* Collection - Collection

### Outputs:
* New Collection - Collection

## Delete Empty Rows by Column
WARNING: Only works if target column is of type Text/String!

### Inputs:
* Collection - Collection
* Column Index - Number

### Ouputs:
* New Collection - Collection

## Delete Empty Columns
Deletes columns where all data is blank or empty

### Inputs:
* Collection - Collection

### Outputs:
* New Collection - Collection

## Delete Non-Empty Rows by Column
WARNING: Only works if target column is type Text/String!

### Inputs:
* Collection - Collection
* Column Index - Number

### Outputs:
* New Collection - Collection

## Delete Column by Name
Deletes a column with a specified name

### Inputs:
* Old Collection - Collection
* Column Name - Text

### Outputs:
* New Collection - Collection

## Rename Column
Renames a single column of a given collection

### Inputs:
* Old Collection - Collection
* Column Name - Text
* New Name - Text

### Outputs:
* New Collection - Text

## Export to CSV w/ Custom Delimiter
Exports a collection to a CSV file with a custom-specified delimiter

### Inputs:
* Collection - Collection
* Target File - Text
* Delimiter - Text

### Outputs:
N/A

## Import CSV w/ Custom Delimiter
Imports a CSV with a custom-specified delimiter

### Inputs:
* Target file - Text
* Delimiter - Text
* Has headers? - Flag

### Outputs:
* Collection - Collection

## Left Outer Join
Performs an equivilant of a left outer join operation between two collections

### Inputs:
* Left Collection - Collection
* Right Collection - Collection
* Key Field - Text

### Outputs:
* Collection Out - Collection

## Reorder Columns
Reorders columns in a target collection based on CSV input of column names

### Inputs:
* Column Order CSV - Text
* Source Collection - Collection

### Outputs:
* Reordered Collection - Collection
