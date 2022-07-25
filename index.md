# Hunter College Advanced CS Education Certificate Portfolio
## CSCI 70900: Programming In a High-Level Language
### Conway's Game of Life Animation
![Picture of Conway's Game of Life Simulation](cgolPicture.png "Animation of Conway's Game of Life")

See the code [here](https://replit.com/@mthomas42/cohort-3-summer-work-marieke-thomas#programming/3/extra/AnimateCgol.java). (Do 
*java AnimateCgolDriver* to see the animation run in the console)

### SuperArray
[This project](https://replit.com/@mthomas42/cohort-3-summer-work-marieke-thomas#programming/6/sa/SuperArray.java) creates from scratch a class called SuperArray (similar to Java's built-in ArrayList class).

## CSCI 70300 – Data Structures in a High Level Language
### Improved Binary Search
Here is Java code that will perform a binary search on an increasing ArrayList and return the *first* index where the target value occurs. Note that an ordinary binary search will return an index where the target occurs but not necessarily the first (for the simplest case, imagine an array list of five threes, [3, 3, 3, 3, 3]. If you search for 3, an ordinary binary search will yield index 2, whereas this method will yield position 0).

```
public int binarySearchGetFirst(int value){

	// create assign variables  representing the high, low and middle indices 
	// while we're not done:
	//   if the item is at data.get(middle), return middle
	//   otherwise, update high, low, and middle
      int low = 0;
      int high = data.size()-1;
      int middle = (low + high)/2;
      while(!(low>high)){
        middle = (low + high)/2;
        if (data.get(middle) == value){
          break;
        } else if (data.get(middle)> value){
          high = middle-1;
        } else if (data.get(middle) < value){
          low = middle + 1;
        }
        if (low > high){
          return -1;
        }
      }
       while (true){
         if (middle != 0 && data.get(middle) == data.get(middle-1)){
           middle --;
         } else{
           return middle;
         }
       }
	    
    }
```

## SEDC 71900 – Methods I: Advanced Study of Secondary Learning Environments for Teaching Computer Science
### CS Unplugged Activity: Be the Code

[This unplugged activity](https://replit.com/@mthomas42/cohort-3-summer-work-marieke-thomas#methods/04_unplugged.md) allows students to act out code to improve their understanding of control flow in Python. An exerpt of the pseudocode is shown below:

```
  if input > 5:
     Stand up (on the floor)
     hop on one foot 3 times
     if input == 7:
       Pat your head
       if input < 7:
         Spin in a circle
   
     if input < 7:
       High five a neighbor
```

## Some CS Jokes
* What is it called when computer programmers taunt and make fun of each other on social media? It is called cyber boolean!
* Why was the computer programmer, who was a Pokemon fanatic, very upset about his Pokemon evolving? Because he expected Char-mander to evolve into a String-mander and not Charmelion!
