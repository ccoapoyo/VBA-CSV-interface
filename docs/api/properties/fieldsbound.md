---
title: fieldsBound
parent: Properties
grand_parent: API
nav_order: 7
---

# fieldsBound
{: .d-inline-block }

New
{: .label .label-purple }

Gets the regular bound of the vectors in the result array on the current instance.
{: .fs-4 .fw-300 }

---

## ReadWrite

_ReadOnly_

---

## Syntax

*expression*.`fieldsBound`

### Parameters

_None_

### Returns

*Type*: `Long`

>📝**Note**
>{: .text-grey-lt-000 .bg-green-000 }
>The `fieldsBound` property returns the number of fields the header record has. Is assumed to the most of the records in the result array has the same number of fields. In an irregular result array will exist at least one record with a number of fields greater or less than the value hold by this property.
{: .text-grey-dk-300 .bg-grey-lt-000 }

See also
: [item property](https://ws-garcia.github.io/VBA-CSV-interface/api/properties/item.html), [rectangularResults property](https://ws-garcia.github.io/VBA-CSV-interface/api/properties/rectangularresults.html).

[Back to Properties overview](https://ws-garcia.github.io/VBA-CSV-interface/api/properties/)