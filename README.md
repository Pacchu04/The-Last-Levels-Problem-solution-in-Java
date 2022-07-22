# The-Last-Levels-Problem-solution-in-Java


Chef is playing a videogame, and is getting close to the end. He decides to finish the rest of the game in a single session.

There are XX levels remaining in the game, and each level takes Chef YY minutes to complete. To protect against eye strain, Chef also decides that every time he completes 33 levels, he will take a ZZ minute break from playing. Note that there is no need to take this break if the game has been completed.

How much time (in minutes) will it take Chef to complete the game?


/* package codechef; // don't place package name! */

import java.util.*;
import java.lang.*;
import java.io.*;
import java.util.Scanner;
/* Name of the class has to be "Main" only if the class is public. */
class Codechef
{
	public static void main (String[] args) throws java.lang.Exception
	{
		Scanner s=new Scanner(System.in);
		int t=s.nextInt();
		while(t!=0){
		    int x=s.nextInt();
		    int y=s.nextInt();
		    int z=s.nextInt();
		    int m=0;
		    int res=0;
		    if(x>3){
		        if(x%3==0){
		            m=(x/3)-1;
		        }
		        else{
		            m=x/3;
		        }
		    res=x*y+(z*m);
		    System.out.println(res);
		    
		}
		else{
		    res=x*y;
		    System.out.println(res);
		}
		t--;
	}
	}
}

