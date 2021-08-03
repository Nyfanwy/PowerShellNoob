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

I'm going to cover multiple ways to create an array with custom column headers and data that can be populated via variables.


```Powershell
[System.Collections.ArrayList]$Array = @()
$value = [PSCustomObject]@{'Column1'="Data";'Column2'="OtherData"}
$Array.Add($value) | Out-Null
```
