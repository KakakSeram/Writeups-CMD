# Check Office License

Press Windows+R key, type `cmd` and press Enter.

## Office 2016, 2019, 2021

* For 64bit system

	```
	cd %ProgramFiles%\Microsoft Office\Office16
	```

* For 32bit system

	```
	cd %ProgramFiles(x86)%\Microsoft Office\Office16
	```

## Office 2013

* For 64bit system

	```
	cd %ProgramFiles%\Microsoft Office\Office15
	```

* For 32bit system

	```
	cd %ProgramFiles(x86)%\Microsoft Office\Office15
	```

## Script Check

```
cscript ospp.vbs /dstatus
```