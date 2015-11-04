# Addition Game
let us make a math game. The user will be asked a simple math problem in the first round. 
For example, to add two single digit numbers. If the user gets this correct, 
they will be given points and asked a more difficult math problem in round 2, 
such as adding a pair of two digit numbers. They will receive more points
and be asked more difficult questions in the following round for every correct answer. 
Every incorrect answer will be followed by a simpler question. There should be a total of 4 rounds. 
At the end of 4 rounds, the code should print the final score. This will be a little challenging, 
so it is the only problem this week. You may need case statements and the random method.

## Java Code
```java
import java.util.Scanner;
public class Addition_Game {
	public static void main(String[] args) {
	
		int score = 0;
		int hardness = 10;
		
		// Round 1
		//	Generate 2 random numbers
		int numberOne = (int)(Math.random() * hardness);
		
		int numberTwo = (int)(Math.random() * hardness);
		
		int correctAnswer = numberOne + numberTwo;
		
		//  Ask the user to add these two numbers together
		System.out.println
		("What integer is " + numberOne + " + " + numberTwo + "?");
		System.out.println("Please answer in integers only.");
		
		//  Read in their response
		Scanner input = new Scanner(System.in);
		int studentAnswer = input.nextInt();
		//  Check if the answer was correct
		//		IF correct
		if (studentAnswer == correctAnswer){
			//			Tell them it was correct
			System.out.println("Answer was correct");
			//			Give them points
			score += hardness;
			System.out.println("Score is: " + score);
			//			Make the next question harder
			hardness *= 10;	
			System.out.println("hardness is: " + hardness);
		}
		//		IF not correct
		else{
			//			Tell them it was wrong
			System.out.println("Answer was not correct");
			// 			Tell them the correct answer
			System.out.println("The correct answer was: " + correctAnswer);
			//			Do not give them points
			score += 0;
			//			Make the next question easier
			if(hardness>10){
				hardness /= 10;	
			}
		}
		System.out.println("End of round 1");
		// end of round 1
		
		// Round 2 
		//	Generate 2 random numbers
		numberOne = (int)(Math.random() * hardness);
		numberTwo = (int)(Math.random() * hardness);

		
		correctAnswer = numberOne + numberTwo;
		
		//  Ask the user to add these two numbers together
		System.out.println
		("What integer is " + numberOne + " + " + numberTwo + "?");
		System.out.println("Please answer in integers only.");
		
		//  Read in their response
		//Scanner input = new Scanner(System.in);
		studentAnswer = input.nextInt();
		//  Check if the answer was correct
		//		IF correct
		if (studentAnswer == correctAnswer){
			//			Tell them it was correct
			System.out.println("Answer was correct");
			//			Give them points
			score += hardness;
			System.out.println("Score is: " + score);
			//			Make the next question harder
			hardness *= 10;	
			System.out.println("hardness is: " + hardness);
		}
		//		IF not correct
		else{
			//			Tell them it was wrong
			System.out.println("Answer was not correct");
			// 			Tell them the correct answer
			System.out.println("The correct answer was: " + correctAnswer);
			//			Do not give them points
			score += 0;
			//			Make the next question easier
			if(hardness>10){
				hardness /= 10;	
			}
		}
		// end of round 2
		System.out.println("End of round 2");
		// Round 3 
		//	Generate 2 random numbers
		numberOne = (int)(Math.random() * hardness);
		numberTwo = (int)(Math.random() * hardness);

		correctAnswer = numberOne + numberTwo;
		
		//  Ask the user to add these two numbers together
		System.out.println
		("What integer is " + numberOne + " + " + numberTwo + "?");
		System.out.println("Please answer in integers only.");
		
		//  Read in their response
		//Scanner input = new Scanner(System.in);
		studentAnswer = input.nextInt();
		//  Check if the answer was correct
		//		IF correct
		if (studentAnswer == correctAnswer){
			//			Tell them it was correct
			System.out.println("Answer was correct");
			//			Give them points
			score += hardness;
			System.out.println("Score is: " + score);
			//			Make the next question harder
			hardness *= 10;	
			System.out.println("hardness is: " + hardness);
		}
		//		IF not correct
		else{
			//			Tell them it was wrong
			System.out.println("Answer was not correct");
			// 			Tell them the correct answer
			System.out.println("The correct answer was: " + correctAnswer);
			//			Do not give them points
			score += 0;
			//			Make the next question easier
			if(hardness>10){
				hardness /= 10;	
			}
		}
		// end of round 3
		System.out.println("End of round 3");
		// Round 4 
		//	Generate 2 random numbers
		numberOne = (int)(Math.random() * hardness);
		numberTwo = (int)(Math.random() * hardness);

		correctAnswer = numberOne + numberTwo;
		
		//  Ask the user to add these two numbers together
		System.out.println
		("What integer is " + numberOne + " + " + numberTwo + "?");
		System.out.println("Please answer in integers only.");
		
		//  Read in their response
		//Scanner input = new Scanner(System.in);
		studentAnswer = input.nextInt();
		//  Check if the answer was correct
		//		IF correct
		if (studentAnswer == correctAnswer){
			//			Tell them it was correct
			System.out.println("Answer was correct");
			//			Give them points
			score += hardness;
			System.out.println("Score is: " + score);
			//			Make the next question harder
			hardness *= 10;	
			System.out.println("hardness is: " + hardness);
		}
		//		IF not correct
		else{
			//			Tell them it was wrong
			System.out.println("Answer was not correct");
			// 			Tell them the correct answer
			System.out.println("The correct answer was: " + correctAnswer);
			//			Do not give them points
			score += 0;
			//			Make the next question easier
			if(hardness>10){
				hardness /= 10;	
			}
		}
		// end of round 4
		System.out.println("End of round 4 and the end of the game");
	}
}
```

## Console Output
```
What integer is 1 + 2?
Please answer in integers only.
3
Answer was correct
Score is: 10
hardness is: 100
End of round 1
What integer is 20 + 83?
Please answer in integers only.
103
Answer was correct
Score is: 110
hardness is: 1000
End of round 2
What integer is 600 + 659?
Please answer in integers only.
1259
Answer was correct
Score is: 1110
hardness is: 10000
End of round 3
What integer is 9258 + 4301?
Please answer in integers only.
13559
Answer was correct
Score is: 11110
hardness is: 100000
End of round 4 and the end of the game

```


## Conclusion
```
Here we discus about the program. In this program we really focused on user inputs and if statements. This easily allowed us to be able to go in and make the program run differently each time no matter how the user enter the data. It was a pretty difficult assignment though it took me quite a bit of time understanding the basics of how the if statements worked. Im really glad we went through git and learned how to use the basics of it. Git allowed me to be able to look in at the master code to figure out things when I was stuck making the program.
```
