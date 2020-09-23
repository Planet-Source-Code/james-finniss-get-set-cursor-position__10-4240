<div align="center">

## get / set cursor position


</div>

### Description

basically this is a quick function to show you how to set or get the position of your mouse cursor.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[James Finniss](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/james-finniss.md)
**Level**          |Beginner
**User Rating**    |4.0 (20 globes from 5 users)
**Compatibility**  |VB\.NET
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__10-1.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/james-finniss-get-set-cursor-position__10-4240/archive/master.zip)





### Source Code

Private Function setCursor(ByVal X As Integer, ByVal Y As Integer)<br>
If Not X = Nothing And Not Y = Nothing Then<br>
Dim curPoint As New Point(0, 0)<br>
curPoint.X = X<br>
curPoint.Y = Y<br>
Cursor.Position = curPoint<br>
End If<br>
End Function<br><br>
Public Function getCursor()<br>
Dim curPoint As New Point(0, 0)<br>
curPoint.X = Cursor.Position.X<br>
curPoint.Y = Cursor.Position.Y<br>
Return curPoint<br>
End Function<br>
'USAGE:<br>
'to get cursor position:<br>
MsgBox(getCursor.x & ", " & getCursor.y)<br>
'to set cursor position:<br>
setCursor(x coordinate, y coordinate)<br><br>
<b>i hope this snippet has helped anyone out there who is strugling with cursor functions.</b>

