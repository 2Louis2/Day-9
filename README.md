# Day-9
Rolling Dice Revised with Loops

//Die Class

public class Die {
	
	protected final int MAX = 6;
	private int faceValue;

	public Die()
	{
	    faceValue = 1;
	}

	public int roll()
	{
	    faceValue = (int)(Math.random() * MAX) + 1;
	    return faceValue;
	}

	public void setFaceValue (int value)
	{
	    faceValue = value;
	}

	public int getFaceValue() {
	    // TODO Auto-generated method stub
	    return faceValue;
	}

}


//Rolling Dice Class

public class RollingDice {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
       
		int sum = 0;
		int twoRepeats = 0;
		int threeRepeats = 0;
		int fourRepeats = 0;
		int fiveRepeats = 0;
		int sixRepeats = 0;
		int sevenRepeats = 0;
		int eightRepeats = 0; 
		int nineRepeats = 0;
		int tenRepeats = 0;
		int elevenRepeats = 0;
		int twelveRepeats = 0;
		int loops = 0;
   
		
		while (loops < 1000 )
				
		{
		
		Die die1, die2;
		int d1, d2;

		die1 = new Die();
		die2 = new Die();

		//Die die3 = new Die ();

		d1 = die1.roll();
		d2 = die2.roll();

		System.out.println ("Die One: " + d1 + ", Die Two: " + d2);

		sum = die1.getFaceValue() + die2.getFaceValue();
		System.out.println ("Sum: " + sum);
				
		if ( sum == 2)
		{
			twoRepeats++;
			loops++;
		}
		   else if (sum == 3)
		   		{
			   		threeRepeats++;
			   		loops++;
		   		}
		   			else if (sum == 4)
		   				{
		   					fourRepeats++;
		   					loops++;
		   				}
		   			     else if (sum == 5)
		   			     	  {
		   			    	 	 fiveRepeats++;
		   			    	 	 loops++;
		   			     	  }
		   			     		else if (sum == 6)
		   			     			{
		   			     				sixRepeats++;
		   			     				loops++;
		   			     			}
		   			     				else if (sum == 7)
		   			     					{
		   			     						sevenRepeats++;
		   			     						loops++;
		   			     					}
		   			     						else if (sum == 8)
		   			     							{
		   			     								eightRepeats++;
		   			     								loops++;
		   			     							}
		   			     								else if (sum == 9)
		   			     								{
		   			     									nineRepeats++;
		   			     									loops++;
		   			     								}
		   			     									else if (sum == 10)
		   			     										{
		   			     											tenRepeats++;
		   			     											loops++;
		   			     										}
		   			     											else if (sum == 11)
		   			     												{
		   			     													elevenRepeats++;
		   			     													loops++;
		   			     												}
		   			     													else if (sum == 12)
		   			     														{
		   			     															twelveRepeats++;
		   			     															loops++;
		   			     														}
		
		System.out.println("");
		
		}
		
		System.out.println("");
		System.out.println("This looped " + loops + " times.");
		System.out.println("");
		System.out.println("Two appeared " + twoRepeats + " times.");
		System.out.println("Three appeared " + threeRepeats + " times.");
		System.out.println("Four appeared " + fourRepeats + " times.");
		System.out.println("Five appeared " + fiveRepeats + " times.");
		System.out.println("Six appeared " + sixRepeats + " times.");
		System.out.println("Seven appeared " + sevenRepeats + " times.");
		System.out.println("Eight appeared " + eightRepeats + " times.");
		System.out.println("Nine appeared " + nineRepeats + " times.");
		System.out.println("Ten appeared " + tenRepeats + " times.");
		System.out.println("Eleven appeared " + elevenRepeats + " times.");
		System.out.println("Twelve appeared " + twelveRepeats + " times.");
				
		
	}

}
