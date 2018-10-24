---
title: Server2003Param.AlternateDatabaseRecoveryPath field (Microsoft.Isam.Esent.Interop.Server2003)
TOCTitle: AlternateDatabaseRecoveryPath field
ms:assetid: F:Microsoft.Isam.Esent.Interop.Server2003.Server2003Param.AlternateDatabaseRecoveryPath
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/microsoft.isam.esent.interop.server2003.server2003param.alternatedatabaserecoverypath(v=EXCHG.10)
ms:contentKeyID: 55104217
ms.date: 07/30/2014
mtps_version: v=EXCHG.10
f1_keywords:
- Microsoft.Isam.Esent.Interop.Server2003.Server2003Param.AlternateDatabaseRecoveryPath
dev_langs:
- CSharp
- JScript
- VB
- other
api_name: 
- Microsoft.Isam.Esent.Interop.Server2003.Server2003Param.AlternateDatabaseRecoveryPath
topic_type: 
- kbSyntax
- apiref
api_type: 
- Managed
api_location: 
- Microsoft.Isam.Esent.Interop.dll
ROBOTS: INDEX,FOLLOW

---

# Server2003Param.AlternateDatabaseRecoveryPath field

The full path to each database is persisted in the transaction logs at run time. Ordinarily, these databases must remain at the original location for transaction replay to function correctly. This parameter can be used to force crash recovery or a restore operation to look for the databases referenced in the transaction log in the specified folder.

**Namespace:**  [Microsoft.Isam.Esent.Interop.Server2003](hh557147\(v=exchg.10\).md)  
**Assembly:**  Microsoft.Isam.Esent.Interop (in Microsoft.Isam.Esent.Interop.dll)

## Syntax

``` vb
'Declaration
Public Const AlternateDatabaseRecoveryPath As JET_param
'Usage
Dim value As JET_param

value = Server2003Param.AlternateDatabaseRecoveryPath
```

``` csharp
public const JET_param AlternateDatabaseRecoveryPath
```

## See also

#### Reference

[Server2003Param class](dn335279\(v=exchg.10\).md)

[Server2003Param members](dn335280\(v=exchg.10\).md)

[Microsoft.Isam.Esent.Interop.Server2003 namespace](hh557147\(v=exchg.10\).md)
