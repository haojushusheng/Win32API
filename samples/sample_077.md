
# Retrieving national language settings

## Before you begin:
See also:

* [LanguageBar ActiveX control](sample_000.md)  
* [Saving available locale records into a cursor](sample_076.md)  
* [Switching between keyboard layouts](sample_275.md)  
  
***  


## Code:
```foxpro  
DO declare

? "System Default LangID:", GetSystemDefaultLangID()
? "User Default LangID:", GetUserDefaultLangID()

? "System Default LCID:", GetSystemDefaultLCID()
? "User Default LCID:", GetUserDefaultLCID()

? "Current Thread Locale:", GetThreadLocale()

? "OEM code-page identifier:", GetOEMCP()
? "ANSI code-page identifier:", GetACP()
? "Current code page (should be the same as GetOEMCP): ",;
	GetKBCodePage()

PROCEDURE declare
	DECLARE SHORT GetThreadLocale IN kernel32
	DECLARE SHORT GetSystemDefaultLangID IN kernel32
	DECLARE SHORT GetUserDefaultLangID IN kernel32
	DECLARE SHORT GetSystemDefaultLCID IN kernel32
	DECLARE SHORT GetUserDefaultLCID IN kernel32
	DECLARE INTEGER GetOEMCP IN kernel32
	DECLARE INTEGER GetACP IN kernel32
	DECLARE INTEGER GetKBCodePage IN user32  
```  
***  


## Listed functions:
[GetACP](../libraries/kernel32/GetACP.md)  
[GetKBCodePage](../libraries/user32/GetKBCodePage.md)  
[GetOEMCP](../libraries/kernel32/GetOEMCP.md)  
[GetSystemDefaultLCID](../libraries/kernel32/GetSystemDefaultLCID.md)  
[GetSystemDefaultLangID](../libraries/kernel32/GetSystemDefaultLangID.md)  
[GetThreadLocale](../libraries/kernel32/GetThreadLocale.md)  
[GetUserDefaultLCID](../libraries/kernel32/GetUserDefaultLCID.md)  
[GetUserDefaultLangID](../libraries/kernel32/GetUserDefaultLangID.md)  