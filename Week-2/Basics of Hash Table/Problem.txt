Question:

![Basics of Hash Table](https://user-images.githubusercontent.com/71627585/151708358-c02fe0d2-590b-4a76-98c3-23de9f891c43.png)



Solution:
import java.util.*;

class TestClass{

 public static void main(String args[] ) throws Exception{

     Scanner sc = new Scanner(System.in);

     int count=0;

     int n= sc.nextInt();

     int [] array= new int[n];

     for(int m=0;m<n;m++){

         array[m]=sc.nextInt();

     }

     //System.out.println(Arrays.toString(array));

   

   HashMap<Integer,Integer> map1=new HashMap<Integer,Integer>();

     for(int i=0;i<array.length;i++)  {

         int ans=array[i]+((i+1)*(i+1));

         int index=(i+1);

         map1.put(index,ans);

     }

     

   HashMap<Integer,Integer> map2=new HashMap<Integer,Integer>();

     for(int j=0;j<array.length;j++)  {

         int ans=array[j]-((j+1)*(j+1));

         int index=(j+1);

         map2.put(index,ans);

     }

   for(Map.Entry m1 : map1.entrySet()){  

    for(Map.Entry m2 : map2.entrySet()){    

     if(m1.getValue()==m2.getValue()){

         //System.out.println(m1.getKey()+"and"+m2.getKey());

         count++;    

     }

     }

 }  

System.out.println(count);

}

}
