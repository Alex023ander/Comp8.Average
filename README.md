# Comp8.Average

public static void main(String[] args) {
        
        double sum = 0; //declares variables
	    
      int intNumbers[] = new int[args.length];

	    if (args.length>0) //continues as long as there are command-line arguments
	    {
	        System.out.println("Values: "); //prints values from command-line arguments 

	        for (String value: args)
	        {
	            System.out.print(value + " "); 
	        }

	        for(int i=0; i<intNumbers.length;i++) //parsing
	        {
	          intNumbers[i]=Integer.parseInt(args[i]);
	          sum=sum+intNumbers[i];
	        }

	        System.out.println("");
	        System.out.println("Average: " + sum/args.length); //calculates average

	    }

	    else //prints when there are no command-line arguments
	    {
	        System.out.println("No arguments.");
	    }
        }
}
