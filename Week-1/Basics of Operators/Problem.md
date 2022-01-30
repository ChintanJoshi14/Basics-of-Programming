Question:

![Basics of Operators](https://user-images.githubusercontent.com/71627585/151707825-5fc81272-99e4-439e-a86c-8b636b8dfaf2.png)


Solution:
import java.util.*;

class TestClass {

  public static void main(String args[] ) throws Exception {

    Scanner sc = new Scanner(System.in);
    double d=s.nextInt();

    double oc=s.nextInt();
    double of=s.nextInt();
    double od=s.nextInt();
    double cs=s.nextInt();
    double cb=s.nextInt();
    double cm=s.nextInt();
    double cd=s.nextInt();
    double result_online;
    double result_classic;

    result_online = oc + (d-of)*od ;

    result_classic= cb + (d/cs)*cm + (d*cd);

    if(result_classic>=result_online) {

      System.out.println("Online Taxi");

      System.exit(0);

    } else {

      System.out.println("Classic Taxi");

      System.exit(0);

}



 

}

}
