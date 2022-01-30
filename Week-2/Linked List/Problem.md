Question:

![Linked list](https://user-images.githubusercontent.com/71627585/151708658-200f1d9c-a880-438b-a839-648a6e0b570e.png)



Solution:
import java.util.*;

class TestClass {

public static void main(String args[] ) throws Exception {

Scanner sc = new Scanner(System.in);

int N = sc.nextInt();

Stack<Integer> st = new Stack<>();

for(int i = 0 ; i<N ; i++){

int num = sc.nextInt();

if(num % 2 == 0){

st.push(num);

}else{

if(!st.empty){

while(!st.empty){

System.out.print(st.pop() + " ");

}

}

System.out.print(num + " ");

}}

while(!st.empty){

System.out.println(num + " ");

}
}
