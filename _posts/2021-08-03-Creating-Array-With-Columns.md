# TL;DR

```Powershell
[System.Collections.ArrayList]$Array = @()

$value = [PSCustomObject] @{ 'Column1' = "Data" ; 'Column2' = "OtherData" }

$Array.Add( $value ) | Out-Null
```

---

# Overview

I'm going to cover multiple ways to create an array with custom column headers and data that can be populated via variables.


```Powershell
[System.Collections.ArrayList]$Array = @()
$value = [PSCustomObject]@{'Column1'="Data";'Column2'="OtherData"}
$Array.Add($value) | Out-Null
```
