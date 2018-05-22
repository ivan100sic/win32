---
title: LB\_SETCARETINDEX message
description: Sets the focus rectangle to the item at the specified index in a multiple-selection list box. If the item is not visible, it is scrolled into view.
ms.assetid: '077c2b9b-6c52-49e2-b5be-ab91c067d5b2'
keywords: ["LB_SETCARETINDEX message Windows Controls"]
topic_type:
- apiref
api_name:
- LB_SETCARETINDEX
api_location:
- Winuser.h
api_type:
- HeaderDef
---

# LB\_SETCARETINDEX message

Sets the focus rectangle to the item at the specified index in a multiple-selection list box. If the item is not visible, it is scrolled into view.

## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>

Specifies the zero-based index of the list box item that is to receive the focus rectangle.

Windows�95/Windows�98/Windows�Millennium Edition (Windows�Me) : The *wParam* parameter is limited to 16-bit values. This means list boxes cannot contain more than 32,767 items. Although the number of items is restricted, the total size in bytes of the items in a list box is limited only by available memory.

</dd> <dt>

*lParam* 
</dt> <dd>

If this value is **FALSE**, the item is scrolled until it is fully visible; if it is **TRUE**, the item is scrolled until it is at least partially visible.

</dd> </dl>

## Return value

If an error occurs, the return value is LB\_ERR (-1). Otherwise, LB\_OKAY (0) is returned.

## Remarks

If this message is sent to a single-selection list box that does not contain a selected item, the caret index is set to the item specified by the *wParam* parameter. If the single-selection list box does contain a selected item, the list box returns LB\_ERR.

## Requirements



|                                     |                                                                                                          |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�Vista \[desktop apps only\]<br/>                                                           |
| Minimum supported server<br/> | Windows Server�2003 \[desktop apps only\]<br/>                                                     |
| Header<br/>                   | <dl> <dt>Winuser.h (include Windows.h)</dt> </dl> |



## See also

<dl> <dt>

[**LB\_GETCARETINDEX**](lb-getcaretindex.md)
</dt> </dl>

�

�




