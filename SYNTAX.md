# Hascal Syntax Example

hello world :
```
use "hascal.core";
print("Hello World");
```
variables :
```
use "hascal.core";
int x = 1;
string str = "Hascal";
float pi = 3.14;
bool testBool = true;//or <bool testBool = false;>
char ch = 'h';
```
arrays:
```
int[] ages = 12,13,14,15;
string[] strs = "hello" , "bye" ;
float[] fls = 1.0,1.1,1.3;
bool[] bls = true , false,false;
char[] chs = 'h','a','s','c','a','l'; 

int[3,3] ages2 = 1,2,3,4,5,6;
print(ages2[3,3]);//output : 6
```
read values :
```
use "hascal.core";
int x = 0;
ReadInt("",x);

string str = "";
ReadStr("",str);
```
comments :
```
// this is a single line comment

/*
  this is a multi line comment
*/

Comment "this is a comment";
```
if...else :
```
use "hascal.core";
int x = 1;
if x== 1 then
  print("x==1");
else
  print("x!=1");
end;
```
for loop :
```
use "hascal.core";
int x = 0;
for x=0 to 10 do
  print(x);
end;
```
while loop :
```
use "hsacal.core";
int x = 1;
while x==1 do
  print("loop");
end;
```
functions :
```
use "hascal.core"
function sayHello();
  print("hello");
end;

function ret() as string;
  return "hello";
end;

function ret2(string ss)  as string;
  print(ss);
end;
```
use modules:
```
use "your_module_name";
```
use C code in Hascal :
```
use "hascal.core";
ccode "
printf("this is ccode in hascal");
";
```