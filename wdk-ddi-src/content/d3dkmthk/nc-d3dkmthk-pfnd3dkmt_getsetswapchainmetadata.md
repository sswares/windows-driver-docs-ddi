---
UID: NC:d3dkmthk.PFND3DKMT_GETSETSWAPCHAINMETADATA
title: PFND3DKMT_GETSETSWAPCHAINMETADATA (d3dkmthk.h)
description: Pfnd3dkmtGetsetswapchainmetadata gets swap chain metadata.
ms.assetid: b9b26c3c-4708-4ac6-b7ca-6714c1e1ce2c
ms.date: 10/19/2018
keywords: ["PFND3DKMT_GETSETSWAPCHAINMETADATA callback function"]
f1_keywords:
 - "d3dkmthk/PFND3DKMT_GETSETSWAPCHAINMETADATA"
 - "PFND3DKMT_GETSETSWAPCHAINMETADATA"
req.header: d3dkmthk.h
req.include-header:
req.target-type:
req.target-min-winverclnt:
req.target-min-winversvr:
req.kmdf-ver:
req.umdf-ver:
req.lib:
req.dll:
req.irql: 
req.ddi-compliance:
req.unicode-ansi:
req.idl:
req.max-support:
req.namespace:
req.assembly:
req.type-library: 
topic_type: 
- apiref
api_type: 
- UserDefined
api_location: 
- d3dkmthk.h
api_name: 
- PFND3DKMT_GETSETSWAPCHAINMETADATA
targetos: Windows
ms.custom: RS5
dev_langs:
 - c++
tech.root: display
---

# PFND3DKMT_GETSETSWAPCHAINMETADATA callback function

## -description

Pfnd3dkmtGetsetswapchainmetadata gets swap chain metadata.

## -prototype

```cpp
//Declaration

PFND3DKMT_GETSETSWAPCHAINMETADATA Pfnd3dkmtGetsetswapchainmetadata; 

// Definition

NTSTATUS Pfnd3dkmtGetsetswapchainmetadata 
(
	D3DKMT_GETSETSWAPCHAINMETADATA *
)
{...}

```

## -parameters

### -param Arg1

Pointer to a [D3DKMT_GETSETSWAPCHAINMETADATA](ns-d3dkmthk-_d3dkmt_getsetswapchainmetadata.md) structure.

## -returns

Returns NTSTATUS.


## -remarks




## -see-also
