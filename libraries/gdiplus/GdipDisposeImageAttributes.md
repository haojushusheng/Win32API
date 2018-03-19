
## Function name : GdipDisposeImageAttributes
Group: GDI+ ImageAttributes - Library: gdiplus    
***  


#### Disposes the ImageAttributes object created by GdipCreateImageAttributes function.
***  


## Code examples:
[GDI+: Color Transparency](../../samples/sample_549.md)  

## Declaration:
```foxpro  
GpStatus WINGDIPAPI GdipDisposeImageAttributes(
	GpImageAttributes *imageattr)  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER GdipDisposeImageAttributes IN gdiplus;
	INTEGER imageattr  
```  
***  


## Parameters:
imageattr
[in] Handle to the ImageAttributes object.  
***  


## Return value:
Returns GpStatus value, 0 means success.  
***  
