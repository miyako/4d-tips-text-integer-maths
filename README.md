# 4d-tips-text-integer-maths

## Example

```
  //text-based integer maths

C_LONGINT($a;$b)

$count:=1000

For ($i;1;$count)
  $a:=Random*(Choose((Random%2)=1;1;-1))
  $b:=Random*(Choose((Random%2)=1;1;-1))
  ASSERT(String($a-$b)=Subtraction (String($a);String($b)))
End for 

For ($i;1;$count)
  $a:=Random*(Choose((Random%2)=1;1;-1))
  $b:=Random*(Choose((Random%2)=1;1;-1))
  ASSERT(String($a+$b)=Addition (String($a);String($b)))
End for 

For ($i;1;$count)
  $a:=Random*(Choose((Random%2)=1;1;-1))
  $b:=Random*(Choose((Random%2)=1;1;-1))
  ASSERT(String($a*$b)=Multiplication (String($a);String($b)))
End for 
```
