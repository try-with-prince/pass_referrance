public class ref_pass{
 int a=110;
static int b=20;
      static  int d=100;
      static int e=20;
    //     static{
             
            
    //  System.out.println(" static block"); 
    //  //System.out.println(ref_pass.d);
    //     }

    public static void main(String[] args)
    {

        ref_pass ref = new ref_pass();
         
        ref_pass r1 = new ref_pass();
        // System.out.println(ref.a);
        //  System.out.println(d);//100 (3rd)
        // // System.out.println(ref.d);
        //  System.out.println(r1.b);//20 (4th)
        // // System.out.println(""+ref.a+ref.b);
        
 d=ref.fun(ref);
 System.out.println(d);//a ki value from fun,50
  System.out.println(r1.b);//60 (static) changed from fun 
   e=r1.fun1(r1);
 System.out.println(e);//4th value 
System.out.println(r1.a);//5th value 
System.out.println(ref.a);// 6th value that change in fun


 
//   System.out.println(ref.a);

 //System.out.println(""+d);
    }
    public int fun(ref_pass ref1)
    {
        ref1.a=50;
        ref1.b=60;
     //int c=ref1.a+ref1.b;
     return a;
     
    }
     public int fun1(ref_pass ref1)
    {
        ref1.a=2000;
    System.out.println(b);//3 rd print, value of b(static)
        //System.out.println(a);
     //int c=ref1.a+ref1.b;
     return a;
     
    }
// {
//     System.out.println(b);//20,20(1st,2nd)
// }

}





50
60
60
2000
2000
50
