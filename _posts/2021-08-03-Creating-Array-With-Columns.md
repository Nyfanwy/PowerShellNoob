	```
{
  [System.Collections.ArrayList]$Array = @()
  $value = [PSCustomObject]@{'AppName'=$app;'Cert Expiration Date'=$EndDate}
  $Array.Add($value) | Out-Null
}
```
