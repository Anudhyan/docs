---
Title: 'toDatePeriod()'
Description: 'Parses the ISO-8601 duration representation as a DatePeriod.'
Subjects:
  - 'Date and Time'
  - 'Computer Science'
Tags:
 - 'DatePeriod'
 - 'DateTimePeriod'
 - 'ISO-8601'
CatalogContent:
  - 'learn-kotlin'
  - 'paths/computer-science'
---
 
The **`toDatePeriod`** function parses the ISO-8601 duration representation as a `DatePeriod`. 
The ISO-8601 duration representation is a string that starts with the letter P followed by a sequence of numbers and units. 
The numbers represent the number of units, and the units can be days, weeks, months, years, hours, minutes, or seconds.
For example, the following ISO-8601 duration representations represent one day, one week, one month, and one year, respectively.
The function returns a `DatePeriod` object that represents the parsed duration. 
The DatePeriod object has two properties: start and endInclusive. The start property is the start date of the duration, and the endInclusive property is the end date of the duration, inclusive.

## Syntax

```pseudo
fun String.toDatePeriod(): DatePeriod
```

## Example

The following code creates a DatePeriod object representing one day:

```kotlin
val oneDayPeriod = "P1D".toDatePeriod()
```

The output will be:

```shell
start: 2023-10-31T22:49:32.000Z
endInclusive: 2023-11-01T22:49:32.000Z
```