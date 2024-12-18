PRINT PATTERN  1*2*3*4  9*10*11*12
For any input number N Print the following code – For below code N=4

1*2*3*4
9*10*11*12
5*6*7*8
13*14*15*16
PREREQUISITE:
Basic knowledge in Java programming, usage of loops.

ALGORITHM:
Take input from user i.e number of lines required (N value).
Take two loops one for each line (say ‘i’) and other for each digit in a particular line (say ‘j’). i starts from 1 and j starts from 1.
Take a result variable (say ‘a’) and initialize it with 1.
Here ‘i’ loop is used to access each line from 1 to n and ‘j’ loop is used to print values in each line. Entire pattern is divided in to even and odd lines. For odd lines it is printed sequentially and for even lines ‘a’ value is incremented by n.
Print ‘a’ value along with * and post increment  until the j loop reaches a value less than n.
Print the final value ‘a’ of each line.
Repeat the ‘i’ loop until it reaches n.
CODE IN JAVA:
[code language=”java”]
import java.lang.*;
import java.io.*;
class Pattern
{
public static void main(String[] args)throws IOException
{
BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
int n,i,j,a=1,t;
System.out.print("Enter N value:");
n=Integer.parseInt(br.readLine());
for(i=1;i<=n;i++)
{
if(i%2==0)
{
t=a+n;
for(j=1;j<n;j++)
{
System.out.print((t++)+"*");
}
System.out.println(t++);
}
else
{
for(j=1;j<n;j++)
{
System.out.print((a++)+"*");
}
System.out.println(a++);
}
}
}
}
[/code]

 

TAKING INPUT:


DISPLAYING OUTPUT:


 
