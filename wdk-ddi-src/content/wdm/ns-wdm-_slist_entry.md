---
UID: NS:wdm._SLIST_ENTRY
title: _SLIST_ENTRY (wdm.h)
description: An SLIST_ENTRY structure describes an entry in a sequenced singly linked list.
old-location: kernel\slist_entry.htm
tech.root: kernel
ms.assetid: 690bcd8a-3c4f-4254-99c7-4ad600b4ae4f
ms.date: 04/30/2018
keywords: ["SLIST_ENTRY structure"]
ms.keywords: "*PSLIST_ENTRY, PSLIST_ENTRY, PSLIST_ENTRY structure pointer [Kernel-Mode Driver Architecture], SLIST_ENTRY, SLIST_ENTRY structure [Kernel-Mode Driver Architecture], _SLIST_ENTRY, kernel.slist_entry, kstruct_d_2bfe90ad-ee2e-4dbf-a028-5b3481aa8695.xml, wdm/PSLIST_ENTRY, wdm/SLIST_ENTRY"
req.header: wdm.h
req.include-header: Wdm.h, Ntddk.h, Ntifs.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
targetos: Windows
req.typenames: SLIST_ENTRY, *PSLIST_ENTRY
f1_keywords:
 - _SLIST_ENTRY
 - wdm/_SLIST_ENTRY
 - PSLIST_ENTRY
 - wdm/PSLIST_ENTRY
 - SLIST_ENTRY
 - wdm/SLIST_ENTRY
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Wdm.h
api_name:
 - SLIST_ENTRY
---

# _SLIST_ENTRY structure


## -description

An <b>SLIST_ENTRY</b> structure describes an entry in a sequenced singly linked list.

## -struct-fields

### -field Next

Pointer to the next entry in the list, or <b>NULL</b> if there is no next entry in the list.

## -remarks

A driver can access the <b>Next</b> member of a <b>SLIST_ENTRY</b>, but must only be updated by the system routines supplied for this purpose.

On 64-bit platforms, <b>SLIST_ENTRY</b> structures must be 16-byte aligned. Drivers can use DECLSPEC_ALIGN(MEMORY_ALLOCATION_ALIGNMENT) to ensure the proper alignment of <b>SLIST_ENTRY</b>.

For more information about how to use <b>SLIST_ENTRY</b> structures to implement a sequenced singly linked list, see <a href="/windows-hardware/drivers/kernel/singly-and-doubly-linked-lists">Singly and Doubly Linked Lists</a>.

## -see-also

<a href="/windows-hardware/drivers/ddi/wdm/nf-wdm-exinterlockedflushslist">ExInterlockedFlushSList</a>



<a href="/windows-hardware/drivers/ddi/wdm/nf-wdm-exinterlockedpopentryslist">ExInterlockedPopEntrySList</a>



<a href="/windows-hardware/drivers/ddi/wdm/nf-wdm-exinterlockedpushentryslist">ExInterlockedPushEntrySList</a>