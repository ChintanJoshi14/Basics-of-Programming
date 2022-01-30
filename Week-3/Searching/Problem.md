Question:

![Searching](https://user-images.githubusercontent.com/71627585/151709069-75499a06-5f81-40e3-a654-ed8e2e586d61.png)

Solution:

import java.io.BufferedReader;
import java.io.InputStreamReader;

import java.util.*;


class TestClass {
    public static void main(String args[] ) throws Exception {
       

        Scanner s = new Scanner(System.in);
        BufferedReader br =new BufferedReader(new InputStreamReader(System.in));

// read input

String str ="";

try{

str = br.readLine();

}

catch(Exception e){}

String input[] = str.trim().split("\\s+");

int x = Integer.parseInt(input[0]);

int y = Integer.parseInt(input[1]);

int s = Integer.parseInt(input[2]);

int t = Integer.parseInt(input[3]);

int count = 0;

// traverse through each point from (x,y) to (x+s , y+s) and if we can reach at that point from given second we will increment count

for(int i = x ; i <= x+s ; i++){

for(int j = y ; j <= y+s ; j++){

if((i+j) <= t){

count++;

}

}

}

System.out.println(count);

       

    }
}
