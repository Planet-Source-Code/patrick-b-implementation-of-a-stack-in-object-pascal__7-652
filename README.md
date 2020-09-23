<div align="center">

## implementation of a stack in Object Pascal


</div>

### Description

A stack coded in Object Pascal. Works with FreePascal and Delphi.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Patrick B\.^](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/patrick-b.md)
**Level**          |Beginner
**User Rating**    |4.1 (29 globes from 7 users)
**Compatibility**  |Delphi 5
**Category**       |[Data Structures](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/data-structures__7-33.md)
**World**          |[Delphi](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/delphi.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/patrick-b-implementation-of-a-stack-in-object-pascal__7-652/archive/master.zip)





### Source Code

```
{ implementation of a stack in Object Pascal
  written by Jared Bruni
  www.LostSideDead.com
}
program stack;
{$APPTYPE CONSOLE}
uses
 SysUtils;
var
array_stack: array [0..255] of string;
pos: integer = 0;
s: string;
i: integer;
procedure push(str: string);
begin
array_stack[pos] := str;
inc(pos);
end;
function pop(): string ;
begin
dec(pos);
result := array_stack[pos];
end;
function get(at: integer): string;
begin
result := array_stack[at];
end;
function size(): integer;
begin
result := pos;
end;
begin
push('hello');
push('world');
push('stack');
push('in pascal');
push(':)');
for i := 0 to size() do begin
writeln(get(i));
end;
read(s);
end.
```

