// # Representing-the-number-of-matching-pair

import java.util.Arrays;
public class matching_pair {

	public static void main(String[] args)
	{
		int arr[]= {20,10,10,40,50,10,20,30,10,50,20};
		int c=0 ;
		int pair=0 ;
		Arrays.sort(arr);			
		int i=0 ;
		  do{
			for(int j=0 ; j<arr.length ; j++)
			{
			 if(arr[i]==arr[j])	 
				{
					c++;
				}
			}
			 if(c>1)
	    		{
    				pair+=(c/2) ;
				}
			      i+=c ;
				c=0;
			}while(i<arr.length);
		 
			System.out.println("Total pair :"+pair);	
	}	

}
