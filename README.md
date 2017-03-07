# pramilamaskar95.github.io
import java.io.*;
import java.util.*;

class Simple
{
	public static void main(String args[])throws Exception
	{
		BufferedReader br=new BufferedReader(new InputStreamReader(System.in));
		String str=br.readLine();
		String ss=" ",s=" ";
		String []ss1=new String[50];
		String []s1=new String[50];
		if(str.indexOf(".")<str.indexOf("?"))
		{
			ss = str.substring(0, str.indexOf("."));
			s=str.substring((str.indexOf(".")+1),str.indexOf("?"));
			ss1=ss.split(" ");
			s1=s.split(" ");
			
		}
		else if(str.indexOf(".")>str.indexOf("?"))
		{
			ss = str.substring(0, str.indexOf("?"));
			s=str.substring((str.indexOf("?")+1),str.indexOf("."));
			ss1=ss.split(" ");
			s1=s.split(" ");
		}
		if(ss1.length>s1.length)
		{
			System.out.println(ss1.length);
		}
		else
		{
			System.out.println(s1.length);
		}
		
		
	}
}
