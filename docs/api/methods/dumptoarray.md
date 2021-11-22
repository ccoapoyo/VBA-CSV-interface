---
title: DumpToArray
parent: Methods
grand_parent: API
nav_order: 5
---

# DumpToArray
{: .fs-9 }

Dumps data from a source, or from the current instance, to an array.
{: .fs-6 .fw-300 }

---

## Syntax

*expression*.`DumpToArray`*(OutPutArray, \[DataSource:= `Nothing`\])*

### Parameters

<table>
<thead>
<tr>
<th style="text-align: left;">Part</th>
<th style="text-align: left;">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align: left;"><em>OutPutArray</em></td>
<td style="text-align: left;">Required. Identifier specifying a dynamic <code>Variant</code> Type array variable.</td>
</tr>
<tr>
<td style="text-align: left;"><em>DataSource</em></td>
<td style="text-align: left;">Optional. Identifier specifying a <code>CSVArrayList</code> object variable representing the data to copy from.</td>
</tr>
</tbody>
</table>

### Returns value

_None_

>📝**Note**
>{: .text-grey-lt-000 .bg-green-000 }
>Before dump data, is required to make a call to the `ImportFromCSV` or `ImportFromCSVstring` method. The *OutPutArray* parameter must be declared as dynamic `Variant` type array. If user forget to do this, an error can occur.
{: .text-grey-dk-300 .bg-grey-lt-000 }

See also
: [ImportFromCSV method](https://ws-garcia.github.io/VBA-CSV-interface/api/methods/importfromcsv.html), [ImportFromCSVstring method](https://ws-garcia.github.io/VBA-CSV-interface/api/methods/importfromcsvstring.html).

---

## Behavior

When the *DataSource* parameter is omitted the `DumpToArray` method makes a copy of all data stored in the current instance. If the user specified a data source, its data is copied and returned in the *OutPutArray* parameter.

>⚠️**Caution**
>{: .text-grey-lt-000 .bg-green-000 }
>The data is always returned in a Two-dimensional array, even when the imported file only contain a field per record.
{: .text-grey-dk-300 .bg-yellow-000 }

[Back to Methods overview](https://ws-garcia.github.io/VBA-CSV-interface/api/methods/)
