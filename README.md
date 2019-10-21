# Converting-IP-address-yo-equivalent-decimal
package find_solutions;

import java.util.Scanner;
import java.util.StringTokenizer;

public class solutions {


	public static void main(String args[])
	{	
		Scanner sc=new Scanner(System.in);
		String s=sc.nextLine();
		String as[]=new String[s.length()];
		
		String num1=null;
		 String rem1=null;
		int rem=0,num=0;
		String result="0x";
		
		for(int i=0;i<1;i++)
		{
			StringTokenizer t=new StringTokenizer(s,".");
			while(t.hasMoreElements())
			{
				as[i]=t.nextToken();

			int temp=Integer.parseInt(as[i]);
		
			if(temp>9)
			{
				num=temp/16;
			   num1=String.valueOf(num);
			    rem=temp%16;
				 rem1=String.valueOf(rem);
				
			if(num>9)
			{
					switch(num)
					{
					
				    case 10:if(num==10)
					{
						result=result+'A';
					}
				    break;
							
					case 11:if(num==11)
					{
						result=result+'B';
					}
					break;
					case 12:if(num==12)
					{
						result=result+'C';
					}
					break;
					case 13:if(num==13)
					{
						result=result+'D';
					}
					break;
					case 14:if(num==14)
					{
						result=result+'E';
					}
					break;
					case 15:if(num==15)
					{
						result=result+'A';
					}
					break;
					
					}
				}
			
			if(num>0 && num<=9)
			{
				
			result=result+num1;
			}
			
			
			
			if(rem>9)
			{
					switch(rem)
					{
					
				    case 10:if(rem==10)
					{
						result=result+'A';
					}
				    break;
							
					case 11:if(rem==11)
					{
						result=result+'B';
					}
					break;
					case 12:if(rem==12)
					{
						result=result+'C';
					}
					break;
					case 13:if(rem==13)
					{
						result=result+'D';
					}
					break;
					case 14:if(rem==14)
					{
						result=result+'E';
					}
					break;
					case 15:if(rem==15)
					{
						result=result+'A';
					}
					break;
					
					}
				}

			if(rem>0 && rem<=9)
			{
				
			result=result+rem1;

			}
		
		}

		}


		}
		System.out.println(result);

	}
}
