---
title: Windows8Api.JetTryPrereadIndexRanges method  (Microsoft.Isam.Esent.Interop.Windows8)
TOCTitle: 'JetTryPrereadIndexRanges method '
ms:assetid: M:Microsoft.Isam.Esent.Interop.Windows8.Windows8Api.JetTryPrereadIndexRanges(Microsoft.Isam.Esent.Interop.JET_SESID,Microsoft.Isam.Esent.Interop.JET_TABLEID,Microsoft.Isam.Esent.Interop.Windows8.JET_INDEX_RANGE[],System.Int32,System.Int32,System.Int32@,Microsoft.Isam.Esent.Interop.JET_COLUMNID[],Microsoft.Isam.Esent.Interop.Windows8.PrereadIndexRangesGrbit)
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.isam.esent.interop.windows8.windows8api.jettryprereadindexranges(v=EXCHG.10)
ms:contentKeyID: 55104421
ms.date: 07/30/2014
ms.topic: reference
f1_keywords:
- Microsoft.Isam.Esent.Interop.Windows8.Windows8Api.JetTryPrereadIndexRanges
dev_langs:
- CSharp
- JScript
- VB
- other
api_name: 
- Microsoft.Isam.Esent.Interop.Windows8.Windows8Api.JetTryPrereadIndexRanges
topic_type: 
- apiref
- kbSyntax
api_type: 
- Managed
api_location: 
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW

---

# Windows8Api.JetTryPrereadIndexRanges method

If the records with the specified key ranges are not in the buffer cache, then start asynchronous reads to bring the records into the database buffer cache.

**Namespace:**  [Microsoft.Isam.Esent.Interop.Windows8](dn335439\(v=exchg.10\).md)  
**Assembly:**  Microsoft.Isam.Esent.Interop (in Microsoft.Isam.Esent.Interop.dll)

## Syntax

``` vb
'Declaration
Public Shared Function JetTryPrereadIndexRanges ( _
    sesid As JET_SESID, _
    tableid As JET_TABLEID, _
    indexRanges As JET_INDEX_RANGE(), _
    rangeIndex As Integer, _
    rangeCount As Integer, _
    <OutAttribute> ByRef rangesPreread As Integer, _
    columnsPreread As JET_COLUMNID(), _
    grbit As PrereadIndexRangesGrbit _
) As Boolean
'Usage
Dim sesid As JET_SESID
Dim tableid As JET_TABLEID
Dim indexRanges As JET_INDEX_RANGE()
Dim rangeIndex As Integer
Dim rangeCount As Integer
Dim rangesPreread As Integer
Dim columnsPreread As JET_COLUMNID()
Dim grbit As PrereadIndexRangesGrbit
Dim returnValue As Boolean

returnValue = Windows8Api.JetTryPrereadIndexRanges(sesid, _
    tableid, indexRanges, rangeIndex, _
    rangeCount, rangesPreread, columnsPreread, _
    grbit)
```

``` csharp
public static bool JetTryPrereadIndexRanges(
    JET_SESID sesid,
    JET_TABLEID tableid,
    JET_INDEX_RANGE[] indexRanges,
    int rangeIndex,
    int rangeCount,
    out int rangesPreread,
    JET_COLUMNID[] columnsPreread,
    PrereadIndexRangesGrbit grbit
)
```

#### Parameters

  - sesid  
    Type: [Microsoft.Isam.Esent.Interop.JET_SESID](hh596745\(v=exchg.10\).md)  
    
    The session to use.

<!-- end list -->

  - tableid  
    Type: [Microsoft.Isam.Esent.Interop.JET_TABLEID](hh566310\(v=exchg.10\).md)  
    
    The table to issue the prereads against.

<!-- end list -->

  - indexRanges  
    Type: \[\]  
    
    The key ranges to preread.

<!-- end list -->

  - rangeIndex  
    Type: [System.Int32](https://docs.microsoft.com/dotnet/api/system.int32?redirectedfrom=MSDN)  
    
    The index of the first key range in the array to read.

<!-- end list -->

  - rangeCount  
    Type: [System.Int32](https://docs.microsoft.com/dotnet/api/system.int32?redirectedfrom=MSDN)  
    
    The maximum number of key ranges to preread.

<!-- end list -->

  - rangesPreread  
    Type: [System.Int32](https://docs.microsoft.com/dotnet/api/system.int32?redirectedfrom=MSDN)  
    
    Returns the number of keys actually preread.

<!-- end list -->

  - columnsPreread  
    Type: \[\]  
    
    List of column ids for long value columns to preread.

<!-- end list -->

  - grbit  
    Type: [Microsoft.Isam.Esent.Interop.Windows8.PrereadIndexRangesGrbit](dn335366\(v=exchg.10\).md)  
    
    Preread options. Used to specify the direction of the preread.

#### Return value

Type: [System.Boolean](https://docs.microsoft.com/dotnet/api/system.boolean?redirectedfrom=MSDN)  
**\[true\]** if some preread done, **\[false\]** otherwise.  

## See also

#### Reference

[Windows8Api class](dn335490\(v=exchg.10\).md)

[Windows8Api members](dn335373\(v=exchg.10\).md)

[Microsoft.Isam.Esent.Interop.Windows8 namespace](dn335439\(v=exchg.10\).md)

