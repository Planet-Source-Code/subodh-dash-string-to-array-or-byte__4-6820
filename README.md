<div align="center">

## String to Array or Byte


</div>

### Description

Converts a string or an integer to an array of characters/bytes
 
### More Info
 
A string or integer

Use it somewhat like this

dim myarray

myarray = StringToArray("324gfsdgfd6,58.kfdsfd//osid")

'You can manipulate myarray as per your wish. The individual elements can be accessed like :

dim p

for p = 0 to ubound(myarray)

msgbox myarray(p)

next

An array


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Subodh Dash](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/subodh-dash.md)
**Level**          |Intermediate
**User Rating**    |5.0 (30 globes from 6 users)
**Compatibility**  |ASP \(Active Server Pages\), VbScript \(browser/client side\)

**Category**       |[Strings](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/strings__4-26.md)
**World**          |[ASP / VbScript](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/asp-vbscript.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/subodh-dash-string-to-array-or-byte__4-6820/archive/master.zip)

### API Declarations

Free to use/distribute


### Source Code

```
Function StringToArray(str_or_int)
 dim l, arr, i
 l = len(str_or_int)
 redim arr(l-1)
 for i = 0 to l-1
 arr(i) = mid(str_or_int,i+1,1)
 next
 StringToArray = arr
end function
```

