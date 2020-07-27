import java.io.*;
import java.util.*;
public class Main
{
    public static char ck (int max , int min,String s1, String s2){
        int i,j,ch=0;
        for(i=max;i>min;i--)
        {
            if(s2.charAt(i)=='Y')
            {
                if(s1.charAt(i-1)=='Y')
                {
                    ch=0;
                }
                else
                {
                    ch=1;
                    break;
                }
            }
            else
            {
                ch=1;
                break;
            }
        }
        
        if(ch==0)
        return 'Y';
        else
        return 'N';
    }
	public static void main(String[] args)throws IOException {
	    BufferedReader br=new BufferedReader (new InputStreamReader(System.in));
	    int i,j,t,n,ck;
	    String s1="",s2="",sn="";
	    t=Integer.parseInt(br.readLine());
	    int t1=t;
	    while(t>0)
	    {
	        t--;
	        n=Integer.parseInt(br.readLine());
	        s1=br.readLine();
	        s2=br.readLine();
	        System.out.println("Case #"+(t1-t)+":");
	        for(i=0;i<n;i++)
	        {
	            int ch=0;
	            int k=0;
	            sn="";
	            if(i==n-1)
	            {
	                while(k<i)
	                {
	                    char ret= ck(i,k,s1,s2);
	                    sn=sn+ret;
                        k++;
	                }
	                sn=sn+'Y';
	            }
	           for(j=i;j<n-1;j++)
	            {  
	                while(k<i)
	                {
	                    char ret= ck(j,k,s1,s2);
	                    sn=sn+ret;
                        k++;
	                }
	                if(ch==0)
	                {
	                    
	                if(i==j)
	                {
	                    sn=sn+'Y';
	                    //continue;
	                    
	                }
	                 if(s2.charAt(j)=='Y')
	                {
	                    if(s1.charAt(j+1)=='Y')
	                    sn=sn+'Y';
	                    else
	                    ch=1;
	                }
	                else
	                ch=1;
	                }
	                if(ch==1)
	                {
	                    
	                    sn=sn+'N';
	                    ch=1;
	                }
	                
	            }
	            System.out.println(sn);
	        }
	    }
	
	}
}
