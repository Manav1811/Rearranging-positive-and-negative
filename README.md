# Rearranging-positive-and-negative
import java.util.Scanner;
public class Main
{
    public static void Rearrangearray(int arr[],int n)
    {
        int a[]=new int[n];
        int i;
        int k=0;
        
        for(i=0;i<n;i++)
         {
             if(arr[i]>=0)
             {
                 a[k++]=arr[i];
             }
         }
         
         for(i=0;i<n;i++)
         {
             if(arr[i]<=0)
             {
                 a[k++]=arr[i];
             }
         }
         
         for(i=0;i<n;i++)
           {
            arr[i]=a[i];
           }
    }
	 
	public static void main(String[] args)
	{
	    int arr[]={2,-1,3,-4,6,7,-8};
	    int n=arr.length;
	    
	    Rearrangearray(arr,n);
	    
	    for (int i=0;i<n;i++)
            System.out.print(arr[i] + " ");
	}

}
