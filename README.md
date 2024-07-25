# menu
Developed a menu of food items using basic java. In this we make menu of   food items by giving amount and prices and users information Using basic java operations
import javax .swing.*;
class restaurant{
 public static void main(String[] args) {
System.out.println("enter name");
String name;
name=JOptionPane.showInputDialog("enter name");
System.out.println(name);
int dob,total4;
dob=Integer.parseInt(JOptionPane.showInputDialog("dob"));
System.out.println(dob);
String num;
        while (true) {
            num = JOptionPane.showInputDialog("Enter phone number");
            if (num.length() == 10 && (num.charAt(0) == '6' || num.charAt(0) == '7' || num.charAt(0) == '8' || num.charAt(0) == '9')) {
                System.out.println(num);
                break;
            } else {
                System.out.println("Wrong number type again");
            }
        }
Integer total1,burger,amt2,total2,total3,amt1,pizza;
pizza=	Integer.parseInt(JOptionPane.showInputDialog("enter quantity of pizza"));
 System.out.println(pizza);

amt1=Integer.parseInt(JOptionPane.showInputDialog("enter amount"));
 System.out.println(amt1);

total1=pizza*amt1;
burger=Integer.parseInt(JOptionPane.showInputDialog("enter quantity of burger"));
amt2=Integer.parseInt(JOptionPane.showInputDialog("enter amount"));
total2=burger*amt2;
total3=total1+total2;
int discount1,discount2;
if(dob%2==0){
discount1=total3*5/100;
}
else{
discount1=total3*3/100;
}
if(num.charAt(0)=='9'||num.charAt(0)=='7'){
discount2=total3*5/100;
}
else if(num.charAt(0)=='6'||num.charAt(0)=='8'){
discount2=total3*2/100;
}
else{
 System.out.println("no discount based on mobile number");
 discount2=0;
}
total4=total3-discount1-discount2;


  
System.out.println("                        welcome                                                   dob:"+dob);
System.out.println(name + "     " + num + "                                                                      27-06-2024");
System.out.println("------------------------------------------------------------------------------------------");

System.out.println("1.pizza             "+pizza+"                     "+amt1+"                        "+total1);
System.out.println("2. burger           "+burger+"                    "+amt2+"                        "+ total2);
System.out.println("                                                                          total amt is  "+total3);
System.out.println("                                                                  discount based on dob  "+discount1);
System.out.println("                                                             discount based on mobile no  "+discount2);


                                                                                          System.out.println("                                                                               ------------");
    
System.out.println("                                                                                 pay"+total4);
}  
}
