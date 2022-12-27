
import java.util.*;

public class Main
{

    public static void Shrijaycount(double[] Price, int Budget, String[] NewsPaper)
    {
 
     
        for (int i = 0; i < Price.length; i++)
            for (int j = i + 1; j < Price.length; j++)
                if ((Price[i] + Price[j]) <= Budget){
                      
                       
                     System.out.print("{"+ NewsPaper[i]+","+ NewsPaper[j]+"}");
                     System.out.print(",");
                }
                
       
    }

	public static void main(String[] args) {

		  
		  String[] NewsPaper = {"TOI", "Hindu", "ET", "BM", "HT"};
		 double[] Price = {26, 20.5, 34, 10.5, 18};
		    
		    Scanner sc = new Scanner(System.in);
		    int Budget = sc.nextInt();
		    Shrijaycount(Price,Budget,NewsPaper);

	}
}
