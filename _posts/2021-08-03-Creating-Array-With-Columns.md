# TL;DR

```Powershell
# Create empty array in $Array variable
  [System.Collections.ArrayList]$Array = @()

# $Value is populated with the column name and the data that will be added under that column name.
  $value = [PSCustomObject] @{ 'Column1' = "Data" ; 'Column2' = "OtherData" }

# We need to add $value into the empty Array, this command appends the $Value so each time you run it, the values will be added again
  $Array.Add( $value ) | Out-Null
```
### Result

![ArrayExample1](/img/ArrayExample1.jpg)

---

# Overview

This Guide will help to cover multiple ways of creating an array within PowerShell.
Specifically, it will cover custom made arrays where you're able to set the column name as well as the data.


```Powershell
[System.Collections.ArrayList]$Array = @()
$value = [PSCustomObject]@{'Column1'="Data";'Column2'="OtherData"}
$Array.Add($value) | Out-Null
```
