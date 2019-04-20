# Partial Date
This module provides date and time fields that allows any individual component 
to be left blank, while still providing a sortable listing of the fields. Useful 
if you need to handle dates like "8:46 a.m Sep 11, 2001 EST", 
"12 noon 25 May, Early 16th Century" or "May 20000 BC" in the one field.

## Installation
See the [relevant section of Drupal 
documentation](https://www.drupal.org/docs/7/extend/installing-modules).

## Feeds Support
This module includes support for Feeds (generously contributed by the Agile 
Humanities Agency).

When configuring a Feeds importer for an entity that contains a partial date, 
the Mappings section will contain Partial Date components that you can select as 
targets. 

These can include the following:
* my partial date field: Approximate (bool)
* my partial date field: Long text description
* my partial date field: Short text description
* my partial date field: from: year
* my partial date field: from: year
* my partial date field: from: year
* my partial date field: from: year - estimate
* my partial date field: from: month
* my partial date field: from: month - estimate
* my partial date field: from: day
* my partial date field: from: day - estimate
* my partial date field: from: hour
* my partial date field: from: hour - estimate
* my partial date field: from: minute
* my partial date field: from: minute - estimate
* my partial date field: from: second
* my partial date field: from: second - estimate
* my partial date field: from: timezone
* my partial date field: to: year
* my partial date field: to: year - estimate
* my partial date field: to: month
* my partial date field: to: month - estimate
* my partial date field: to: day
* my partial date field: to: day - estimate
* my partial date field: to: hour
* my partial date field: to: hour - estimate
* my partial date field: to: minute
* my partial date field: to: minute - estimate
* my partial date field: to: second
* my partial date field: to: second - estimate
* my partial date field: to: timezone

Not all of the above components will be available in the list. "To" components 
only exist if this field is of type Partial Date Range. Also, only the elements 
that are enabled for this field instance will be accessible. Configure this at 
Admin > Structure > Content types > [my content type]. 

A Partial date field can be set up with customized labels for range estimates. 
For example, the years 1500 to 1599 may be called "16th century". The feeds 
importer checks for labels, so values that can be imported (e.g. the column in 
your CSV) may be "1500|1599" or "16th century" to the same effect. Please note 
that they are case sensitive. If the label is not recognized the value will not 
be imported.

To import months, please use the numeric value, i.e. either "02" or "2" for 
February.
