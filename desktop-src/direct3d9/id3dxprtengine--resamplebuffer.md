---
Description: Resamples an input ID3DXPRTBuffer buffer and saves it to an output buffer. This method can be used to convert a vertex buffer to a texture buffer and vice-versa. It can also be used to convert single-channel buffers to 3-channel buffers and vice-versa.
ms.assetid: 78015044-38a9-4c08-a690-28f6427dae8c
title: ID3DXPRTEngine::ResampleBuffer method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# ID3DXPRTEngine::ResampleBuffer method

Resamples an input [**ID3DXPRTBuffer**](id3dxprtbuffer.md) buffer and saves it to an output buffer. This method can be used to convert a vertex buffer to a texture buffer and vice-versa. It can also be used to convert single-channel buffers to 3-channel buffers and vice-versa.

## Syntax


```C++
HRESULT ResampleBuffer(
  [in]      LPD3DXPRTBUFFER pBufferIn,
  [in, out] LPD3DXPRTBUFFER pBufferOut
);
```



## Parameters

<dl> <dt>

*pBufferIn* \[in\]
</dt> <dd>

Type: **[**LPD3DXPRTBUFFER**](id3dxprtbuffer.md)**

Pointer to the input [**ID3DXPRTBuffer**](id3dxprtbuffer.md) buffer.

</dd> <dt>

*pBufferOut* \[in, out\]
</dt> <dd>

Type: **[**LPD3DXPRTBUFFER**](id3dxprtbuffer.md)**

Pointer to the output [**ID3DXPRTBuffer**](id3dxprtbuffer.md) buffer.

</dd> </dl>

## Return value

Type: **[**HRESULT**](https://msdn.microsoft.com/en-us/library/Bb401631(v=MSDN.10).aspx)**

If the method succeeds, the return value is S\_OK. If the method fails, the return value can be one of the following: D3DERR\_INVALIDCALL, E\_OUTOFMEMORY.

## Requirements



|                    |                                                                                        |
|--------------------|----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX9Mesh.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>   |



## See also

<dl> <dt>

[ID3DXPRTEngine](id3dxprtengine.md)
</dt> </dl>

 

 



