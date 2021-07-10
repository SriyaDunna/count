# count
import java.util.*;
public class strProgram
{
   public static void main(String args[])
   {
    String str;
    int i,l_alph,u_alph,digi,spl;
    l_alph=0;
    u_alph=0;
    digi=0;
    spl=0;
    char ch;
    int count=0;
    int count1=0;
    Scanner sc=new Scanner (System.in);
    System.out.print("Enter string:");
    str=sc.nextLine();
    for(i=0;i<str.length();i++)
    {
       ch=str.charAt(i);
       if(ch>='a'&&ch<='z')
       {
       l_alph++;
       }
    else if(ch>='A'&&ch<='Z')
     {
      u_alph++;
     }
     else if(ch>='0'&&ch<='9')
        digi++;
     else 
       spl++;
    }
    if(l_alph==u_alph)
    {
     count=count+1;
     }
     if(digi==spl)
     count = count + 1;
     if(count==count1){
    System.out.print("Yes");
     }
    else
    System.out.print("No");
  }
}
