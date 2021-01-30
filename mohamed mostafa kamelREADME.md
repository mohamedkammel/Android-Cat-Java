# Android-Cat-Java

package task2;


public class cylinder 
{
    final double pi = 3.14 ;
    
    public double volumeOfCylinder(int a , int b)
    {
        int r = a;
        int h = b;
        double volume = pi*r*r*h ;
        return volume;
    }
    public double areaOfCylinder(int r , int h)
    {
        double area = (2*pi*r*r)+(2*pi*r*h) ;
        return area;
    
    }
}


package task2;


public class circle extends cylinder 
{
    public double areaOfCircle(int r)
    {
        double area = pi*r*r ;
        return area;
    }
    
}



package task2;

public class Task2 {

    public static void main(String[] args) 
    {
        double result;
        
      circle x = new circle();
      
      result = x.volumeOfCylinder(10, 34);
      System.out.println(result);
      
      result = x.areaOfCylinder(2, 9);
      System.out.println(result);
      
     result = x.areaOfCircle(314);
     System.out.println(result);
     
      
      
    }
