# javapdf
















CA LAB-IV (A) LAB on Java Programming Assignments 
Assignment 1) Write a program that demonstrate program structure of java with use of 
arithmetical and logical implementation. 
public class Assignment1  
{ 
public static void main(String[] args)  
{ 
} 
} 
// initializing variables 
int num1 = 20, num2 = 10, sum = 0,diff = 0,multi=0; 
float div=0; 
System.out.println("num1 = " + num1); 
System.out.println("num2 = " + num2); 
sum = num1 + num2; 
System.out.println("The sum = " + sum); 
diff = num1 - num2; 
System.out.println("The diff = " + diff); 
multi = num1 * num2; 
System.out.println("The multi = " + multi); 
div = num1 / num2; 
System.out.println("The div = " + div); 
if ((num1==20) && (num2==10))// You can also use || operator 
{ 
} 
System.out.println("Both True"); 
else 
System.out.println("Both Not True"); 
OUTPUT:- 
num1 = 20  num2 = 10  The sum = 30 The diff = 10 The multi = 200 The div = 2.0 Both True 
1 
2 
 
Assignment 2) Write a program that demonstrate string operations using String and 
StringBuffer class. 
package assignment2; 
import java.io.*; 
public class Assignment2  
{ 
    public static void main(String[] args)  
    { 
        try 
      { 
           DataInputStream d= new DataInputStream(System.in);                 
            System.out.println("\n enter the 1st String  "); 
            String s=d.readLine(); 
            //String Functions 
            int y=s.length(); 
     System.out.println("\n length of string is "+y); 
       String z=s.toUpperCase(); 
    System.out.println("\n string in upper case "+z); 
      String l=s.toLowerCase(); 
    System.out.println("\n string in lower  case "+l); 
    char m=s.charAt(3); 
    System.out.println("\n char at 3rd index is  "+m); 
    String o=s.replace('a','b'); 
    System.out.println("\n replaced string is "+o); 
    String n=s.substring(2,5); 
    System.out.println("\n sub string from 2 to 5 index  is  "+n); 
    System.out.println("\n enter the character to find index"); 
    String s2=d.readLine(); 
           int a=s.indexOf(s2); 
     System.out.println("\n index of char is "+a); 
3 
 
           System.out.println("\n enter the character to find last index"); 
    String s3=d.readLine(); 
   int b=s.lastIndexOf(s3); 
   System.out.println("\n last index of char is  "+b); 
          System.out.println("\n enter the 2nd String "); 
          String s1=d.readLine(); 
      String p=s.concat(s1); 
   System.out.println("\n concated string is "+p); 
   boolean b1=s.equals(s1); 
   if(b1==true) 
   { 
              System.out.println("\n strings are equal "); 
   } 
   else 
   { 
                System.out.println("\n strings are  not equal "); 
   } 
          //StringBuffer  Functions 
          StringBuffer sf = new StringBuffer("Coding Atharva"); 
          System.out.println("\n String = "+sf); // Will Print the string 
          System.out.println("\n Length = "+sf.length() ); // total numbers of characters    
          System.out.println("\n Length = "+sf.capacity() ); // total allocated capacity 
          sf.setLength(6); // Sets the length and destroy the remaining characters  
         System.out.println("\n After setting length String = "+sf); 
         sf.setCharAt(0,'K'); // It will change character at specified position 
        System.out.println("\n SetCharAt String = "+sf); 
          sf.setCharAt(0,'C'); 
          int a1 = 7; 
            sf.append(a1); // It concatenates the other data type value 
        System.out.println("\n Appended String = "+sf); 
sf.insert(6," Atharva"); // used to insert one string or char or object 
System.out.println("\n Inserted String = "+sf); 
sf.reverse();   
System.out.println("\n Reverse String = "+sf); 
} 
} 
} 
catch(Exception e) 
{ 
} 
OUTPUT:- 
enter the 1st String   
manojkumar 
length of string is 10 
System.out.println(""+e); 
string in upper case MANOJKUMAR 
string in lower  case manojkumar 
char at 3rd index is  o 
replaced string is mbnojkumbr 
sub string from 2 to 5 index  is  noj 
enter the character to find index 
a 
index of char is 1 
enter the character to find last index 
a 
last index of char is  8 
enter the 2nd String  
sonawane 
concated string is manojkumarsonawane 
4 
strings are  not equal  
String = Coding Atharva 
Length = 14 
Length = 30 
After setting length String = Coding 
SetCharAt String = Koding 
Appended String = Coding7 
Inserted String = Coding Atharva7 
Reverse String = 7avrahtA gnidoC 
5 
Assignment 3) Write a program that demonstrate inner class and static fields. 
package assignment3; 
class Outer  
{ 
{ 
} 
} 
int outer_x = 100;  
void test()  
{ 
} 
Inner inner = new Inner(); inner.display(); 
static int count=0;//will get memory only once and retain its value   
Outer() 
{   
} 
count++;//incrementing the value of static variable   
System.out.println(count);   
class Inner  
void display()  
{ 
} 
System.out.println("display: outer_x = " + outer_x); 
public class Assignment3  
{ 
public static void main(String[] args)  
{ 
Outer outer = new Outer();  
outer.test(); 
6 
//creating objects   
Outer o1=new Outer();   
Outer o2=new Outer();   
Outer o3=new Outer();   
} 
} 
OUTPUT:- 
1 
display: outer_x = 100 
2 
3 
4 
7 
Assignment 4) Write a program that demonstrate inheritance, polymorphism. 
package assignment4; 
class Animal 
{  
} 
public void move() 
{ 
} 
System.out.println("Animals can move"); 
class Dog extends Animal 
{  
} 
//Method Overriding 
public void move() 
{ 
} 
System.out.println("Dogs can walk and run"); 
//Method Overloading 
void add(int a,int b) 
{ 
} 
int s=a+b; 
System.out.println("Sum="+s); 
void add(int a,int b,int c) 
{ 
} 
int s=a+b+c; 
System.out.println("Sum="+s); 
public class Assignment4  
8 
{ 
public static void main(String[] args)  
{ 
} 
} 
Animal a =new Animal();  
Animal b =new Dog();  
a.move(); 
b.move(); 
Dog d=new Dog();  
d.add(10,20); 
d.add(10,20,30); 
OUTPUT:- 
Animals can move 
Dogs can walk and run 
Sum=30 
Sum=60 
9 
Assignment 5) Write a program that demonstrate 2D shapes on frames. 
Steps:- 
1. Right Click on your project- New-JFrame  
2. Drag JPanel on JFrame 
3. Drag JButtons on JPanel 
4. Right Click on JButtons-Edit Text 
5. Right Click on JButtons-Events-select event/methods you want and write appropriate 
code. 
6. Code 
package assignment5; 
import java.awt.*; 
import java.awt.geom.*; 
public class NewJFrame extends javax.swing.JFrame { 
public NewJFrame() { 
initComponents(); 
} 
@SuppressWarnings("unchecked") 
// <editor-fold defaultstate="collapsed" desc="Generated Code">                           
private void initComponents() { 
jPanel1 = new javax.swing.JPanel(); 
jButton1 = new javax.swing.JButton(); 
jButton2 = new javax.swing.JButton(); 
jButton4 = new javax.swing.JButton(); 
setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE); 
jButton1.setText("Rectangle"); 
jButton1.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jButton1ActionPerformed(evt); 
} 
}); 
jButton2.setText("Ellipse"); 
jButton2.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jButton2ActionPerformed(evt); 
} 
}); 
jButton4.setText("Line"); 
jButton4.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jButton4ActionPerformed(evt); 
} 
}); 
10 
javax.swing.GroupLayout jPanel1Layout = new 
javax.swing.GroupLayout(jPanel1); 
jPanel1.setLayout(jPanel1Layout); 
jPanel1Layout.setHorizontalGroup( 
jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addContainerGap() 
.addComponent(jButton1) 
.addGap(18, 18, 18) 
.addComponent(jButton2) 
.addGap(18, 18, 18) 
.addComponent(jButton4) 
.addContainerGap(92, Short.MAX_VALUE)) 
); 
jPanel1Layout.setVerticalGroup( 
jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addGap(27, 27, 27) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
BASELINE) 
.addComponent(jButton1) 
.addComponent(jButton2) 
.addComponent(jButton4)) 
.addContainerGap(228, Short.MAX_VALUE)) 
); 
javax.swing.GroupLayout layout = new 
javax.swing.GroupLayout(getContentPane()); 
getContentPane().setLayout(layout); 
layout.setHorizontalGroup( 
layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(layout.createSequentialGroup() 
.addContainerGap() 
.addComponent(jPanel1, javax.swing.GroupLayout.PREFERRED_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addContainerGap(59, Short.MAX_VALUE)) 
); 
layout.setVerticalGroup( 
layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(layout.createSequentialGroup() 
.addContainerGap() 
.addComponent(jPanel1, javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE) 
11 
12 
 
                .addContainerGap()) 
        ); 
 
        pack(); 
    }// </editor-fold>                         
    private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here: 
        Graphics g1=jPanel1.getGraphics(); 
        Graphics2D g2  = (Graphics2D)g1; 
 g2.setPaint(Color.ORANGE); 
        double leftx=100; 
        double topy=100; 
        double width=100; 
 double height=200;//For Squre width and height should be same 
        Rectangle2D rect = new 
Rectangle2D.Double(leftx,topy,leftx+width,topy+height); 
 g2.fill(rect); 
      
    }                                         
    private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here: 
         Graphics g1=jPanel1.getGraphics(); 
        Graphics2D g2  = (Graphics2D)g1; 
 g2.setPaint(Color.CYAN); 
        double leftx=300; 
        double topy=100; 
        double width=30; 
 double height=40;//For Circle width and height should be same 
        Ellipse2D ellipse = new Ellipse2D.Double(leftx,topy,width,height); 
 g2.fill(ellipse); 
    }                                         
    private void jButton4ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here: 
         Graphics g1=jPanel1.getGraphics(); 
        Graphics2D g2  = (Graphics2D)g1; 
 g2.setPaint(Color.MAGENTA); 
        double startx=50; 
        double starty=60; 
        double endx=600; 
 double endy=600; 
        Line2D line = new Line2D.Double(startx,starty,endx,endy); 
 g2.draw(line);  
    }                                         
    public static void main(String args[]) { 
        /* Set the Nimbus look and feel */ 
        //<editor-fold defaultstate="collapsed" desc=" Look and feel setting code 
(optional) "> 
/* If Nimbus (introduced in Java SE 6) is not available, stay with the default look 
and feel. 
* For details see 
http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html  
*/ 
try { 
for (javax.swing.UIManager.LookAndFeelInfo info : 
javax.swing.UIManager.getInstalledLookAndFeels()) { 
if ("Nimbus".equals(info.getName())) { 
javax.swing.UIManager.setLookAndFeel(info.getClassName()); 
break; 
} 
} 
} catch (ClassNotFoundException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (InstantiationException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (IllegalAccessException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (javax.swing.UnsupportedLookAndFeelException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} 
//</editor-fold> 
/* Create and display the form */ 
java.awt.EventQueue.invokeLater(new Runnable() { 
public void run() { 
new NewJFrame().setVisible(true); 
} 
}); 
} 
// Variables declaration - do not modify                      
private javax.swing.JButton jButton1; 
private javax.swing.JButton jButton2; 
private javax.swing.JButton jButton4; 
private javax.swing.JPanel jPanel1; 
// End of variables declaration                    
} 
7. Right Click in Code-Run File 
13 
14 
 
OUTPUT:- 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
Assignment 6) Write a program that demonstrate color and fonts. 
Steps:- 
1. Right Click on your project- New-JFrame  
2. Drag JPanel on JFrame 
3. Drag JButton on JPanel 
4. Right Click on JButton-Edit Text 
5. Right Click on JButton-Events-select event/methods you want and write appropriate 
code. 
6. Code 
import java.awt.*; 
import java.awt.geom.*; 
import java.util.*; 
public class NewJFrame extends javax.swing.JFrame { 
public NewJFrame() { 
initComponents(); 
} 
@SuppressWarnings("unchecked") 
// <editor-fold defaultstate="collapsed" desc="Generated Code">                           
private void initComponents() { 
jPanel1 = new javax.swing.JPanel(); 
jButton1 = new javax.swing.JButton(); 
setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE); 
jButton1.setText("Click"); 
jButton1.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jButton1ActionPerformed(evt); 
} 
}); 
javax.swing.GroupLayout jPanel1Layout = new 
javax.swing.GroupLayout(jPanel1); 
jPanel1.setLayout(jPanel1Layout); 
jPanel1Layout.setHorizontalGroup( 
jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addGap(213, 213, 213) 
.addComponent(jButton1) 
.addContainerGap(667, Short.MAX_VALUE)) 
); 
jPanel1Layout.setVerticalGroup( 
jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(jPanel1Layout.createSequentialGroup() 
15 
16 
 
                .addComponent(jButton1) 
                .addGap(0, 578, Short.MAX_VALUE)) 
        ); 
 
        javax.swing.GroupLayout layout = new 
javax.swing.GroupLayout(getContentPane()); 
        getContentPane().setLayout(layout); 
        layout.setHorizontalGroup( 
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
            .addGroup(layout.createSequentialGroup() 
                .addGap(20, 20, 20) 
                .addComponent(jPanel1, javax.swing.GroupLayout.PREFERRED_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
                .addContainerGap(55, Short.MAX_VALUE)) 
        ); 
        layout.setVerticalGroup( 
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
            .addGroup(layout.createSequentialGroup() 
                .addGap(22, 22, 22) 
                .addComponent(jPanel1, javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE) 
                .addContainerGap()) 
        ); 
 
        pack(); 
    }// </editor-fold>                         
 
    private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here: 
        GraphicsEnvironment 
ge=GraphicsEnvironment.getLocalGraphicsEnvironment(); 
 String s[]=ge.getAvailableFontFamilyNames(); 
        Graphics g1=jPanel1.getGraphics(); 
        Random rd = new Random(); 
        
        int y=50; 
        int sz=20; 
  for(int i=0;i<s.length;i++) 
  { 
   Font f=new Font(s[i],Font.BOLD,sz);//Font.ITALIC 
   g1.setFont(f); 
                         
                        int r=rd.nextInt(255); 
                        int g=rd.nextInt(255); 
                        int b=rd.nextInt(255); 
                        Color c=new Color(r,g,b); 
                        g1.setColor(c); 
} 
g1.drawString("Hello World",50,y); 
y=y+20; 
sz=sz+1; 
}                                         
public static void main(String args[]) { 
/* Set the Nimbus look and feel */ 
//<editor-fold defaultstate="collapsed" desc=" Look and feel setting code 
(optional) "> 
/* If Nimbus (introduced in Java SE 6) is not available, stay with the default look 
and feel. 
* For details see 
http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html  
*/ 
try { 
for (javax.swing.UIManager.LookAndFeelInfo info : 
javax.swing.UIManager.getInstalledLookAndFeels()) { 
if ("Nimbus".equals(info.getName())) { 
javax.swing.UIManager.setLookAndFeel(info.getClassName()); 
break; 
} 
} 
} catch (ClassNotFoundException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (InstantiationException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (IllegalAccessException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (javax.swing.UnsupportedLookAndFeelException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} 
//</editor-fold> 
/* Create and display the form */ 
java.awt.EventQueue.invokeLater(new Runnable() { 
public void run() { 
new NewJFrame().setVisible(true); 
} 
}); 
17 
} 
// Variables declaration - do not modify                      
private javax.swing.JButton jButton1; 
private javax.swing.JPanel jPanel1; 
// End of variables declaration                    
} 
7. Right Click in Code-Run File 
OUTPUT:- 
18 
Assignment 7) Write a program to illustrate use of various swing components. 
Steps:- 
1. Right Click on your project- New-JFrame  
2. Drag JPanel on JFrame 
3. Drag various components 
4. Right Click on components-Edit Text 
5. Drag ButtonGroup component and set buttonGroup property of radiobuttons. 
6. Right Click on jComboBox, jList1 and set model property. 
7. Write Code on Button ActionPerformed 
package assignment7; 
public class NewJFrame extends javax.swing.JFrame { 
public NewJFrame() { 
initComponents(); 
} 
@SuppressWarnings("unchecked") 
// <editor-fold defaultstate="collapsed" desc="Generated Code">                           
private void initComponents() { 
buttonGroup1 = new javax.swing.ButtonGroup(); 
jPanel1 = new javax.swing.JPanel(); 
jLabel1 = new javax.swing.JLabel(); 
jTextField1 = new javax.swing.JTextField(); 
jLabel2 = new javax.swing.JLabel(); 
jScrollPane1 = new javax.swing.JScrollPane(); 
jTextArea1 = new javax.swing.JTextArea(); 
jLabel3 = new javax.swing.JLabel(); 
jCheckBox1 = new javax.swing.JCheckBox(); 
jCheckBox2 = new javax.swing.JCheckBox(); 
jCheckBox3 = new javax.swing.JCheckBox(); 
jButton1 = new javax.swing.JButton(); 
jLabel4 = new javax.swing.JLabel(); 
jRadioButton1 = new javax.swing.JRadioButton(); 
jRadioButton2 = new javax.swing.JRadioButton(); 
jLabel5 = new javax.swing.JLabel(); 
jComboBox1 = new javax.swing.JComboBox(); 
jLabel6 = new javax.swing.JLabel(); 
jScrollPane2 = new javax.swing.JScrollPane(); 
jList1 = new javax.swing.JList(); 
setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE); 
jLabel1.setText("Enter Rno"); 
jLabel2.setText("Enter Name"); 
jTextArea1.setColumns(20); 
19 
jTextArea1.setRows(5); 
jScrollPane1.setViewportView(jTextArea1); 
jLabel3.setText("Favorite Color"); 
jCheckBox1.setText("Red"); 
jCheckBox2.setText("Green"); 
jCheckBox3.setText("Blue"); 
jButton1.setText("Click"); 
jButton1.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jButton1ActionPerformed(evt); 
} 
}); 
jLabel4.setText("Class"); 
buttonGroup1.add(jRadioButton1); 
jRadioButton1.setText("MCA-1"); 
buttonGroup1.add(jRadioButton2); 
jRadioButton2.setText("MCA-2"); 
jLabel5.setText("Laptop"); 
jComboBox1.setModel(new javax.swing.DefaultComboBoxModel(new String[] 
{ "HP", "Dell", "Lenovo" })); 
jLabel6.setText("Subject"); 
jList1.setModel(new javax.swing.AbstractListModel() { 
String[] strings = { "C", "C++", "Java" }; 
public int getSize() { return strings.length; } 
public Object getElementAt(int i) { return strings[i]; } 
}); 
jScrollPane2.setViewportView(jList1); 
javax.swing.GroupLayout jPanel1Layout = new 
javax.swing.GroupLayout(jPanel1); 
jPanel1.setLayout(jPanel1Layout); 
jPanel1Layout.setHorizontalGroup( 
jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addGap(35, 35, 35) 
20 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
LEADING) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
TRAILING, false) 
.addComponent(jLabel6, 
javax.swing.GroupLayout.Alignment.LEADING, 
javax.swing.GroupLayout.DEFAULT_SIZE, 62, Short.MAX_VALUE) 
.addComponent(jLabel5, 
javax.swing.GroupLayout.Alignment.LEADING, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)) 
.addGap(44, 44, 44) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
LEADING) 
.addComponent(jComboBox1, 
javax.swing.GroupLayout.PREFERRED_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addComponent(jScrollPane2, 
javax.swing.GroupLayout.PREFERRED_SIZE, 68, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addComponent(jButton1, 
javax.swing.GroupLayout.PREFERRED_SIZE, 92, 
javax.swing.GroupLayout.PREFERRED_SIZE))) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
LEADING) 
.addComponent(jLabel1, 
javax.swing.GroupLayout.PREFERRED_SIZE, 68, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addComponent(jLabel2, 
javax.swing.GroupLayout.PREFERRED_SIZE, 68, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addComponent(jLabel3, 
javax.swing.GroupLayout.PREFERRED_SIZE, 96, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addComponent(jLabel4, 
javax.swing.GroupLayout.PREFERRED_SIZE, 50, 
javax.swing.GroupLayout.PREFERRED_SIZE)) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
LEADING) 
.addGroup(jPanel1Layout.createSequentialGroup() 
21 
.addGap(25, 25, 25) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
LEADING) 
.addComponent(jCheckBox1) 
.addComponent(jCheckBox2) 
.addComponent(jCheckBox3) 
.addComponent(jScrollPane1, 
javax.swing.GroupLayout.PREFERRED_SIZE, 146, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addComponent(jTextField1, 
javax.swing.GroupLayout.PREFERRED_SIZE, 89, 
javax.swing.GroupLayout.PREFERRED_SIZE))) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addGap(13, 13, 13) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
LEADING) 
.addComponent(jRadioButton1) 
.addComponent(jRadioButton2)))))) 
.addContainerGap(691, Short.MAX_VALUE)) 
); 
jPanel1Layout.setVerticalGroup( 
jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addGap(55, 55, 55) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
BASELINE) 
.addComponent(jLabel1, javax.swing.GroupLayout.PREFERRED_SIZE, 
29, javax.swing.GroupLayout.PREFERRED_SIZE) 
.addComponent(jTextField1, 
javax.swing.GroupLayout.PREFERRED_SIZE, 29, 
javax.swing.GroupLayout.PREFERRED_SIZE)) 
.addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
LEADING) 
.addComponent(jScrollPane1, 
javax.swing.GroupLayout.PREFERRED_SIZE, 62, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addComponent(jLabel2, javax.swing.GroupLayout.PREFERRED_SIZE, 
25, javax.swing.GroupLayout.PREFERRED_SIZE)) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
LEADING) 
22 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addGap(12, 12, 12) 
.addComponent(jLabel3, 
javax.swing.GroupLayout.PREFERRED_SIZE, 35, 
javax.swing.GroupLayout.PREFERRED_SIZE)) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addGap(18, 18, 18) 
.addComponent(jCheckBox1) 
.addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED) 
.addComponent(jCheckBox2) 
.addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED) 
.addComponent(jCheckBox3))) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
LEADING) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addGap(21, 21, 21) 
.addComponent(jRadioButton1) 
.addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED) 
.addComponent(jRadioButton2) 
.addGap(23, 23, 23)) 
.addGroup(javax.swing.GroupLayout.Alignment.TRAILING, 
jPanel1Layout.createSequentialGroup() 
.addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED) 
.addComponent(jLabel4, 
javax.swing.GroupLayout.PREFERRED_SIZE, 25, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addGap(36, 36, 36))) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
TRAILING) 
.addComponent(jLabel5, javax.swing.GroupLayout.PREFERRED_SIZE, 
26, javax.swing.GroupLayout.PREFERRED_SIZE) 
.addComponent(jComboBox1, 
javax.swing.GroupLayout.PREFERRED_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.PREFERRED_SIZE)) 
.addGap(18, 18, 18) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
LEADING) 
.addComponent(jLabel6, javax.swing.GroupLayout.PREFERRED_SIZE, 
24, javax.swing.GroupLayout.PREFERRED_SIZE) 
23 
.addComponent(jScrollPane2, 
javax.swing.GroupLayout.PREFERRED_SIZE, 75, 
javax.swing.GroupLayout.PREFERRED_SIZE)) 
.addGap(31, 31, 31) 
.addComponent(jButton1, javax.swing.GroupLayout.PREFERRED_SIZE, 
37, javax.swing.GroupLayout.PREFERRED_SIZE) 
.addContainerGap(64, Short.MAX_VALUE)) 
); 
javax.swing.GroupLayout layout = new 
javax.swing.GroupLayout(getContentPane()); 
getContentPane().setLayout(layout); 
layout.setHorizontalGroup( 
layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(layout.createSequentialGroup() 
.addComponent(jPanel1, javax.swing.GroupLayout.PREFERRED_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addGap(0, 0, Short.MAX_VALUE)) 
); 
layout.setVerticalGroup( 
layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(javax.swing.GroupLayout.Alignment.TRAILING, 
layout.createSequentialGroup() 
.addContainerGap(javax.swing.GroupLayout.DEFAULT_SIZE, 
Short.MAX_VALUE) 
.addComponent(jPanel1, javax.swing.GroupLayout.PREFERRED_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addContainerGap()) 
); 
pack(); 
}// </editor-fold>                         
private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
// TODO add your handling code here: 
System.out.println("Rno= "+jTextField1.getText()); 
System.out.println("Name= "+jTextArea1.getText()); 
String color=" "; 
if (jCheckBox1.isSelected()) 
color=color+" "+jCheckBox1.getText(); 
if (jCheckBox2.isSelected()) 
color=color+" "+jCheckBox2.getText(); 
if (jCheckBox3.isSelected()) 
color=color+" "+jCheckBox3.getText(); 
System.out.println("Favorite Colors= "+color); 
24 
String cl=" "; 
if (jRadioButton1.isSelected()) 
cl=cl+" "+jRadioButton1.getText(); 
else 
cl=cl+" "+jRadioButton2.getText(); 
System.out.println("Class= "+cl); 
System.out.println("Laptop= "+jComboBox1.getSelectedItem().toString()); 
System.out.println("Subjects= "); 
Object o[]=jList1.getSelectedValues(); 
for(int i=0;i<o.length;i++) 
{ 
System.out.println(o[i].toString()); 
} 
}                                         
public static void main(String args[]) { 
/* Set the Nimbus look and feel */ 
//<editor-fold defaultstate="collapsed" desc=" Look and feel setting code 
(optional) "> 
/* If Nimbus (introduced in Java SE 6) is not available, stay with the default look 
and feel. 
* For details see 
http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html  
*/ 
try { 
for (javax.swing.UIManager.LookAndFeelInfo info : 
javax.swing.UIManager.getInstalledLookAndFeels()) { 
if ("Nimbus".equals(info.getName())) { 
javax.swing.UIManager.setLookAndFeel(info.getClassName()); 
break; 
} 
} 
} catch (ClassNotFoundException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (InstantiationException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (IllegalAccessException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (javax.swing.UnsupportedLookAndFeelException ex) { 
25 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} 
//</editor-fold> 
/* Create and display the form */ 
java.awt.EventQueue.invokeLater(new Runnable() { 
public void run() { 
new NewJFrame().setVisible(true); 
} 
}); 
} 
// Variables declaration - do not modify                      
private javax.swing.ButtonGroup buttonGroup1; 
private javax.swing.JButton jButton1; 
private javax.swing.JCheckBox jCheckBox1; 
private javax.swing.JCheckBox jCheckBox2; 
private javax.swing.JCheckBox jCheckBox3; 
private javax.swing.JComboBox jComboBox1; 
private javax.swing.JLabel jLabel1; 
private javax.swing.JLabel jLabel2; 
private javax.swing.JLabel jLabel3; 
private javax.swing.JLabel jLabel4; 
private javax.swing.JLabel jLabel5; 
private javax.swing.JLabel jLabel6; 
private javax.swing.JList jList1; 
private javax.swing.JPanel jPanel1; 
private javax.swing.JRadioButton jRadioButton1; 
private javax.swing.JRadioButton jRadioButton2; 
private javax.swing.JScrollPane jScrollPane1; 
private javax.swing.JScrollPane jScrollPane2; 
private javax.swing.JTextArea jTextArea1; 
private javax.swing.JTextField jTextField1; 
// End of variables declaration                    
} 
8. Right Click in Code-Run File 
OUTPUT:- 
26 
Assignment 8) Write a program that demonstrate use of dialog box and menus. 
Steps:- 
1. Right Click on your project- New-JFrame  
2. Drag JPanel on JFrame 
3. Drag JMenuBar--Edit Text 
4. Right Click on JMenuBar-select Add From Palette-MenuItem/Separator. 
5. Right Click on MenuItem-select event/methods you want. 
6. Drag Popup Menu on JPanel and add MenuItem, event/methods in it similarly. 
7. Right Click on your JPanel, set componentPopupMenu property to your popup 
menu. 
8. For User DialogBox- Drag JDialog on JPanel, Right Click on your JDialog
setLayout, Right Click on your JDialog-Add From Palette-Swing Controls. 
9. Write Following Code 
package assignment8; 
import javax.swing.*; 
import java.io.*; 
import java.awt.*; 
public class NewJFrame extends javax.swing.JFrame { 
public NewJFrame() { 
initComponents(); 
} 
@SuppressWarnings("unchecked") 
// <editor-fold defaultstate="collapsed" desc="Generated Code">                           
private void initComponents() { 
jPopupMenu1 = new javax.swing.JPopupMenu(); 
Red = new javax.swing.JMenuItem(); 
Green = new javax.swing.JMenuItem(); 
Blue = new javax.swing.JMenuItem(); 
jDialog1 = new javax.swing.JDialog(); 
jTextField1 = new javax.swing.JTextField(); 
Click = new javax.swing.JButton(); 
jPanel1 = new javax.swing.JPanel(); 
jMenuBar1 = new javax.swing.JMenuBar(); 
jMenu1 = new javax.swing.JMenu(); 
jMenuItem1 = new javax.swing.JMenuItem(); 
jSeparator1 = new javax.swing.JPopupMenu.Separator(); 
jMenuItem2 = new javax.swing.JMenuItem(); 
jSeparator2 = new javax.swing.JPopupMenu.Separator(); 
jCheckBoxMenuItem1 = new javax.swing.JCheckBoxMenuItem(); 
jSeparator3 = new javax.swing.JPopupMenu.Separator(); 
jRadioButtonMenuItem1 = new javax.swing.JRadioButtonMenuItem(); 
jSeparator5 = new javax.swing.JPopupMenu.Separator(); 
jMenuItem6 = new javax.swing.JMenuItem(); 
jSeparator4 = new javax.swing.JPopupMenu.Separator(); 
27 
jMenuItem4 = new javax.swing.JMenuItem(); 
jMenu2 = new javax.swing.JMenu(); 
jMenuItem3 = new javax.swing.JMenuItem(); 
Red.setText("Red"); 
Red.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
RedActionPerformed(evt); 
} 
}); 
jPopupMenu1.add(Red); 
Green.setText("Green"); 
Green.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
GreenActionPerformed(evt); 
} 
}); 
jPopupMenu1.add(Green); 
Blue.setText("Blue"); 
Blue.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
BlueActionPerformed(evt); 
} 
}); 
jPopupMenu1.add(Blue); 
jDialog1.getContentPane().setLayout(new java.awt.FlowLayout()); 
jTextField1.setText("jTextField1"); 
jDialog1.getContentPane().add(jTextField1); 
Click.setText("Click"); 
jDialog1.getContentPane().add(Click); 
setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE); 
jPanel1.setComponentPopupMenu(jPopupMenu1); 
javax.swing.GroupLayout jPanel1Layout = new 
javax.swing.GroupLayout(jPanel1); 
jPanel1.setLayout(jPanel1Layout); 
jPanel1Layout.setHorizontalGroup( 
jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGap(0, 958, Short.MAX_VALUE) 
); 
jPanel1Layout.setVerticalGroup( 
jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGap(0, 581, Short.MAX_VALUE) 
); 
jMenu1.setText("File"); 
jMenu1.addActionListener(new java.awt.event.ActionListener() { 
28 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jMenu1ActionPerformed(evt); 
} 
}); 
jMenuItem1.setAccelerator(javax.swing.KeyStroke.getKeyStroke(java.awt.event.Key
Event.VK_A, java.awt.event.InputEvent.CTRL_MASK)); 
jMenuItem1.setText("InputDialogBox"); 
jMenuItem1.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jMenuItem1ActionPerformed(evt); 
} 
}); 
jMenu1.add(jMenuItem1); 
jMenu1.add(jSeparator1); 
jMenuItem2.setAccelerator(javax.swing.KeyStroke.getKeyStroke(java.awt.event.Key
Event.VK_B, java.awt.event.InputEvent.CTRL_MASK)); 
jMenuItem2.setText("MessageDialogBox"); 
jMenuItem2.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jMenuItem2ActionPerformed(evt); 
} 
}); 
jMenu1.add(jMenuItem2); 
jMenu1.add(jSeparator2); 
jCheckBoxMenuItem1.setAccelerator(javax.swing.KeyStroke.getKeyStroke(java.awt.
event.KeyEvent.VK_C, java.awt.event.InputEvent.ALT_MASK)); 
jCheckBoxMenuItem1.setSelected(true); 
jCheckBoxMenuItem1.setText("ConfirmDialogBox"); 
jCheckBoxMenuItem1.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jCheckBoxMenuItem1ActionPerformed(evt); 
} 
}); 
jMenu1.add(jCheckBoxMenuItem1); 
jMenu1.add(jSeparator3); 
jRadioButtonMenuItem1.setAccelerator(javax.swing.KeyStroke.getKeyStroke(java.a
wt.event.KeyEvent.VK_D, java.awt.event.InputEvent.SHIFT_MASK)); 
jRadioButtonMenuItem1.setSelected(true); 
jRadioButtonMenuItem1.setText("OptionDialogBox"); 
29 
jRadioButtonMenuItem1.addActionListener(new 
java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jRadioButtonMenuItem1ActionPerformed(evt); 
} 
}); 
jMenu1.add(jRadioButtonMenuItem1); 
jMenu1.add(jSeparator5); 
jMenuItem6.setText("FileChooser"); 
jMenuItem6.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jMenuItem6ActionPerformed(evt); 
} 
}); 
jMenu1.add(jMenuItem6); 
jMenu1.add(jSeparator4); 
jMenuItem4.setText("ColorChooser"); 
jMenuItem4.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jMenuItem4ActionPerformed(evt); 
} 
}); 
jMenu1.add(jMenuItem4); 
jMenuBar1.add(jMenu1); 
jMenu2.setText("Edit"); 
jMenuItem3.setText("UserDialogBox"); 
jMenuItem3.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jMenuItem3ActionPerformed(evt); 
} 
}); 
jMenu2.add(jMenuItem3); 
jMenuBar1.add(jMenu2); 
setJMenuBar(jMenuBar1); 
javax.swing.GroupLayout layout = new 
javax.swing.GroupLayout(getContentPane()); 
getContentPane().setLayout(layout); 
layout.setHorizontalGroup( 
layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(layout.createSequentialGroup() 
.addGap(28, 28, 28) 
.addComponent(jPanel1, javax.swing.GroupLayout.PREFERRED_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addContainerGap(26, Short.MAX_VALUE)) 
30 
31 
 
        ); 
        layout.setVerticalGroup( 
            layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
            .addGroup(layout.createSequentialGroup() 
                .addGap(35, 35, 35) 
                .addComponent(jPanel1, javax.swing.GroupLayout.PREFERRED_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
                .addContainerGap(javax.swing.GroupLayout.DEFAULT_SIZE, 
Short.MAX_VALUE)) 
        ); 
 
        pack(); 
    }// </editor-fold>                         
    private void jMenuItem1ActionPerformed(java.awt.event.ActionEvent evt) {                                           
        // TODO add your handling code here: 
        String n=JOptionPane.showInputDialog("Enter Name"); 
        System.out.println("Name="+n); 
    }                                           
    private void jMenuItem3ActionPerformed(java.awt.event.ActionEvent evt) {                                           
        // TODO add your handling code here: 
        jDialog1.setTitle("This is my DialogBox"); 
        jDialog1.setSize(222,222); 
        jDialog1.show(); 
    }                                           
    private void jMenuItem2ActionPerformed(java.awt.event.ActionEvent evt) {                                           
        // TODO add your handling code here: 
        JOptionPane.showMessageDialog(null,"Success"); 
        
    }                                           
    private void jCheckBoxMenuItem1ActionPerformed(java.awt.event.ActionEvent 
evt) {                                                    
        // TODO add your handling code here: 
        int i=JOptionPane.showConfirmDialog(null, "Are you Sure?"); 
        System.out.println(i); 
    }                                                   
    private void jRadioButtonMenuItem1ActionPerformed(java.awt.event.ActionEvent 
evt) {                                                       
        // TODO add your handling code here: 
        String[] options = {"first", "second", "third"}; 
        int x = JOptionPane.showOptionDialog(null, "Select Option", 
                "OptionDialogBox",JOptionPane.DEFAULT_OPTION, 
JOptionPane.INFORMATION_MESSAGE, null, options, options[0]); 
        System.out.println("Your Option is "+x); 
        
    }                                                      
    private void RedActionPerformed(java.awt.event.ActionEvent evt) {                                     
        // TODO add your handling code here: 
32 
 
        jPanel1.setBackground(Color.red); 
    }                                    
    private void GreenActionPerformed(java.awt.event.ActionEvent evt) {                                       
        // TODO add your handling code here: 
        jPanel1.setBackground(Color.green); 
    }                                      
    private void BlueActionPerformed(java.awt.event.ActionEvent evt) {                                      
        // TODO add your handling code here: 
        jPanel1.setBackground(Color.blue); 
    }                                     
    private void jMenu1ActionPerformed(java.awt.event.ActionEvent evt) {                                        
        // TODO add your handling code here: 
         
    }                                       
    private void jMenuItem6ActionPerformed(java.awt.event.ActionEvent evt) {                                           
        // TODO add your handling code here: 
        JFileChooser fc=new JFileChooser();     
        int i=fc.showOpenDialog(this);     
        if(i==JFileChooser.APPROVE_OPTION) 
        {     
              File f=fc.getSelectedFile();     
             String filepath=f.getPath();     
             System.out.println("You Selected "+filepath); 
        } 
    }                                           
    private void jMenuItem4ActionPerformed(java.awt.event.ActionEvent evt) {                                           
        // TODO add your handling code here: 
        Color c=JColorChooser.showDialog(this,"Select a color",Color.ORANGE);     
        jPanel1.setBackground(c); 
     
    }                                           
    public static void main(String args[]) { 
        /* Set the Nimbus look and feel */ 
        //<editor-fold defaultstate="collapsed" desc=" Look and feel setting code 
(optional) "> 
        /* If Nimbus (introduced in Java SE 6) is not available, stay with the default look 
and feel. 
         * For details see 
http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html  
         */ 
        try { 
            for (javax.swing.UIManager.LookAndFeelInfo info : 
javax.swing.UIManager.getInstalledLookAndFeels()) { 
                if ("Nimbus".equals(info.getName())) { 
                    javax.swing.UIManager.setLookAndFeel(info.getClassName()); 
                    break; 
                } 
            } 
} catch (ClassNotFoundException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (InstantiationException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (IllegalAccessException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (javax.swing.UnsupportedLookAndFeelException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} 
//</editor-fold> 
/* Create and display the form */ 
java.awt.EventQueue.invokeLater(new Runnable() { 
public void run() { 
new NewJFrame().setVisible(true); 
} 
}); 
} 
// Variables declaration - do not modify                      
private javax.swing.JMenuItem Blue; 
private javax.swing.JButton Click; 
private javax.swing.JMenuItem Green; 
private javax.swing.JMenuItem Red; 
private javax.swing.JCheckBoxMenuItem jCheckBoxMenuItem1; 
private javax.swing.JDialog jDialog1; 
private javax.swing.JMenu jMenu1; 
private javax.swing.JMenu jMenu2; 
private javax.swing.JMenuBar jMenuBar1; 
private javax.swing.JMenuItem jMenuItem1; 
private javax.swing.JMenuItem jMenuItem2; 
private javax.swing.JMenuItem jMenuItem3; 
private javax.swing.JMenuItem jMenuItem4; 
private javax.swing.JMenuItem jMenuItem6; 
private javax.swing.JPanel jPanel1; 
private javax.swing.JPopupMenu jPopupMenu1; 
private javax.swing.JRadioButtonMenuItem jRadioButtonMenuItem1; 
private javax.swing.JPopupMenu.Separator jSeparator1; 
private javax.swing.JPopupMenu.Separator jSeparator2; 
private javax.swing.JPopupMenu.Separator jSeparator3; 
private javax.swing.JPopupMenu.Separator jSeparator4; 
33 
private javax.swing.JPopupMenu.Separator jSeparator5; 
private javax.swing.JTextField jTextField1; 
// End of variables declaration                    
} 
10. Right Click in Code-Run File 
OUTPUT:- 
34 
Assignment 9) Write a program that demonstrate event handling for various types of 
events. 
Steps:- 
1. Right Click on your project- New-JFrame  
2. Drag JPanel on JFrame 
3. Drag JButton, JTextField on JPanel 
4. Right Click on JButton, JTextField-Edit Text 
5. Right Click on JButton, JTextField, JPanel-Events-select event/methods you want and 
write appropriate code. 
6. Code 
package assignment9; 
import java.awt.Color; 
public class NewJFrame extends javax.swing.JFrame { 
public NewJFrame() { 
initComponents(); 
} 
@SuppressWarnings("unchecked") 
// <editor-fold defaultstate="collapsed" desc="Generated Code">                           
private void initComponents() { 
jPanel1 = new javax.swing.JPanel(); 
jButton2 = new javax.swing.JButton(); 
jTextField1 = new javax.swing.JTextField(); 
setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE); 
jPanel1.addMouseListener(new java.awt.event.MouseAdapter() { 
public void mouseClicked(java.awt.event.MouseEvent evt) { 
jPanel1MouseClicked(evt); 
} 
}); 
jButton2.setText("Mouse"); 
jButton2.addMouseListener(new java.awt.event.MouseAdapter() { 
public void mouseEntered(java.awt.event.MouseEvent evt) { 
jButton2MouseEntered(evt); 
} 
public void mouseExited(java.awt.event.MouseEvent evt) { 
jButton2MouseExited(evt); 
} 
}); 
jTextField1.addKeyListener(new java.awt.event.KeyAdapter() { 
public void keyTyped(java.awt.event.KeyEvent evt) { 
jTextField1KeyTyped(evt); 
} 
}); 
35 
javax.swing.GroupLayout jPanel1Layout = new 
javax.swing.GroupLayout(jPanel1); 
jPanel1.setLayout(jPanel1Layout); 
jPanel1Layout.setHorizontalGroup( 
jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addGap(53, 53, 53) 
.addComponent(jButton2, javax.swing.GroupLayout.PREFERRED_SIZE, 
112, javax.swing.GroupLayout.PREFERRED_SIZE) 
.addGap(81, 81, 81) 
.addComponent(jTextField1, 
javax.swing.GroupLayout.PREFERRED_SIZE, 95, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addContainerGap(635, Short.MAX_VALUE)) 
); 
jPanel1Layout.setVerticalGroup( 
jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addGap(24, 24, 24) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
BASELINE) 
.addComponent(jButton2, 
javax.swing.GroupLayout.PREFERRED_SIZE, 33, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addComponent(jTextField1, 
javax.swing.GroupLayout.PREFERRED_SIZE, 33, 
javax.swing.GroupLayout.PREFERRED_SIZE)) 
.addContainerGap(541, Short.MAX_VALUE)) 
); 
javax.swing.GroupLayout layout = new 
javax.swing.GroupLayout(getContentPane()); 
getContentPane().setLayout(layout); 
layout.setHorizontalGroup( 
layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(layout.createSequentialGroup() 
.addContainerGap() 
.addComponent(jPanel1, javax.swing.GroupLayout.PREFERRED_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addContainerGap(19, Short.MAX_VALUE)) 
); 
layout.setVerticalGroup( 
layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
36 
37 
 
            .addGroup(layout.createSequentialGroup() 
                .addContainerGap() 
                .addComponent(jPanel1, javax.swing.GroupLayout.PREFERRED_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
                .addContainerGap(28, Short.MAX_VALUE)) 
        ); 
 
        pack(); 
    }// </editor-fold>                         
 
    private void jButton2MouseEntered(java.awt.event.MouseEvent evt) {                                       
        // TODO add your handling code here: 
        jPanel1.setBackground(Color.red); 
    }                                      
    private void jButton2MouseExited(java.awt.event.MouseEvent evt) {                                      
        // TODO add your handling code here: 
         jPanel1.setBackground(Color.GREEN); 
    }                                     
    private void jTextField1KeyTyped(java.awt.event.KeyEvent evt) {                                      
        // TODO add your handling code here: 
         char a=evt.getKeyChar(); 
   if(a=='r' || a=='R') 
   { 
    jPanel1.setBackground(Color.red); 
     
   } 
                        else if(a=='g' || a=='G') 
   { 
     jPanel1.setBackground(Color.GREEN); 
     
   } 
                        else 
                        { 
                                jPanel1.setBackground(Color.BLACK); 
                        } 
    }                                     
 int count=0; 
    private void jPanel1MouseClicked(java.awt.event.MouseEvent evt) {                                      
        // TODO add your handling code here: 
        count++; 
        if(count==1) 
            jPanel1.setBackground(Color.RED); 
        else if(count==2) 
            jPanel1.setBackground(Color.GREEN); 
        else if(count==3) 
            jPanel1.setBackground(Color.BLUE); 
        else 
}                                     
count=0; 
public static void main(String args[]) { 
/* Set the Nimbus look and feel */ 
//<editor-fold defaultstate="collapsed" desc=" Look and feel setting code 
(optional) "> 
/* If Nimbus (introduced in Java SE 6) is not available, stay with the default look 
and feel. 
* For details see 
http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html  
*/ 
try { 
for (javax.swing.UIManager.LookAndFeelInfo info : 
javax.swing.UIManager.getInstalledLookAndFeels()) { 
if ("Nimbus".equals(info.getName())) { 
javax.swing.UIManager.setLookAndFeel(info.getClassName()); 
break; 
} 
} 
} catch (ClassNotFoundException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (InstantiationException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (IllegalAccessException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (javax.swing.UnsupportedLookAndFeelException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} 
//</editor-fold> 
/* Create and display the form */ 
java.awt.EventQueue.invokeLater(new Runnable() { 
public void run() { 
new NewJFrame().setVisible(true); 
} 
}); 
} 
// Variables declaration - do not modify                      
private javax.swing.JButton jButton2; 
38 
} 
private javax.swing.JPanel jPanel1; 
private javax.swing.JTextField jTextField1; 
// End of variables declaration                    
7. Right Click in Code-Run File 
OUTPUT:- 
39 
Assignment 10) Write a program to illustrate multithreading. 
package assignment10; 
class TestSleepMethod1 extends Thread 
{ 
} 
public void run() 
{ 
} 
for(int i=1;i<=5;i++) 
{ 
try 
{ 
} 
System.out.println(i); 
Thread.sleep(500); 
catch(InterruptedException e) 
{ 
} 
} 
System.out.println(e); 
public class Assignment10  
{ 
public static void main(String[] args)  
{ 
TestSleepMethod1 t1=new TestSleepMethod1(); 
TestSleepMethod1 t2=new TestSleepMethod1(); 
TestSleepMethod1 t3=new TestSleepMethod1(); 
t1.start(); 
t2.start(); 
40 
t3.start(); 
} 
} 
OUTPUT:- 
1 
1 
1 
2 
2 
2 
3 
3 
3 
4 
4 
4 
5 
5 
5 
41 
42 
 
Assignment 11) Write a program to illustrate exception handling. 
package assignment11; 
public class Assignment11  
{ 
    public static void main(String[] args)  
    { 
        try 
        { 
            int i=2/0; 
            int a[]=new int[5];  
            a[10]=30; 
        } 
        catch(ArrayIndexOutOfBoundsException e) 
        {    
            System.out.println("ArrayIndexOutOfBoundsException"); 
        } 
        catch(ArithmeticException e) 
        { 
            System.out.println("ArithmeticException"); 
        } 
        catch(Exception e) 
        { 
            System.out.println("Exception"); 
        } 
        finally 
        { 
            System.out.println("Finally"); 
        } 
    } 
  } 
OUTPUT:- 
ArithmeticException 
Finally 
 
 
 
 
 
 
 
 
 
 
Assignment 12) Write a program to demonstrate use of File class. 
package assignment12; 
import java.io.*; 
public class Assignment12  
{ 
public static void main(String[] args)  
{ 
FileInputStream sourceStream = null; //FileReader for char by char 
FileOutputStream targetStream = null; //FileWriter for char by char 
try 
{  
}  
sourceStream= new FileInputStream("sorcefile.txt");  
targetStream= new FileOutputStream("targetfile.txt");  
// Reading source file and writing  
// content to target file byte by byte  
int temp;  
while ((temp = sourceStream.read())!= -1)  
{ 
} 
targetStream.write(temp);  
sourceStream.close();  
targetStream.close();  
catch(Exception e) 
{ 
} 
System.out.println("Exception"); 
//File class 
43 
File f = new File("sorcefile.txt");   
System.out.println("The name of the file is: " + f.getName());   
System.out.println("The absolute path of the file is: " + f.getAbsolutePath());      
System.out.println("Is file writeable?: " + f.canWrite());     
System.out.println("Is file readable " + f.canRead());     
System.out.println("The size of the file in bytes is: " + f.length());   
System.out.println("File Exist "+f.exists()); 
System.out.println("Is File or Directory "+f.isFile()); 
System.out.println("Is File or Directory "+f.isDirectory()); 
System.out.println("Is Hidden "+f.isHidden()); 
System.out.println("Last Modified Time: " + f.lastModified()); 
}   
} 
OUTPUT: 
The name of the file is: sorcefile.txt 
The absolute path of the file is: F:\M.S.Sonawane\2021-22\Java\Assignment12\sorcefile.txt 
Is file writeable?: true 
Is file readable true 
The size of the file in bytes is: 46 
File Exist true 
Is File or Directory true 
Is File or Directory false 
Is Hidden false 
Last Modified Time: 1642157554913 
44 
Assignment 13) Write a program that demonstrate JDBC on application. 
Steps:- 
1. Right Click on your project- New-JFrame  
2. Drag JPanel on JFrame 
3. Drag 2 JLabels, 2 JTextFields, 4 JButtons on JPanel 
4. Right Click on all-Edit Text 
5. Create Database 
6. Create DSN and connect it to Database. 
7. Connect DSN to your application in NetBeans. 
8. Right Click on 4 JButtons-Events-select event/methods you want and write 
appropriate code. 
9. Code 
package assignment13; 
import java.sql.*; 
public class NewJFrame extends javax.swing.JFrame { 
public NewJFrame() { 
initComponents(); 
} 
@SuppressWarnings("unchecked") 
// <editor-fold defaultstate="collapsed" desc="Generated Code">                           
private void initComponents() { 
jPanel1 = new javax.swing.JPanel(); 
jLabel1 = new javax.swing.JLabel(); 
jTextField1 = new javax.swing.JTextField(); 
jLabel2 = new javax.swing.JLabel(); 
jTextField2 = new javax.swing.JTextField(); 
jButton1 = new javax.swing.JButton(); 
jButton2 = new javax.swing.JButton(); 
jButton3 = new javax.swing.JButton(); 
jButton4 = new javax.swing.JButton(); 
setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE); 
jLabel1.setText("RNo"); 
jLabel2.setText("Name"); 
jButton1.setText("Insert"); 
jButton1.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jButton1ActionPerformed(evt); 
} 
}); 
45 
jButton2.setText("Update"); 
jButton2.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jButton2ActionPerformed(evt); 
} 
}); 
jButton3.setText("Delete"); 
jButton3.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jButton3ActionPerformed(evt); 
} 
}); 
jButton4.setText("Select"); 
jButton4.addActionListener(new java.awt.event.ActionListener() { 
public void actionPerformed(java.awt.event.ActionEvent evt) { 
jButton4ActionPerformed(evt); 
} 
}); 
javax.swing.GroupLayout jPanel1Layout = new 
javax.swing.GroupLayout(jPanel1); 
jPanel1.setLayout(jPanel1Layout); 
jPanel1Layout.setHorizontalGroup( 
jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addGap(83, 83, 83) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
LEADING, false) 
.addComponent(jButton1, javax.swing.GroupLayout.DEFAULT_SIZE, 
72, Short.MAX_VALUE) 
.addComponent(jLabel1, javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE) 
.addComponent(jLabel2, javax.swing.GroupLayout.PREFERRED_SIZE, 
53, javax.swing.GroupLayout.PREFERRED_SIZE)) 
.addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.RELATED) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
LEADING) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addComponent(jButton2, 
javax.swing.GroupLayout.PREFERRED_SIZE, 83, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
46 
.addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED) 
.addComponent(jButton3, 
javax.swing.GroupLayout.PREFERRED_SIZE, 81, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addPreferredGap(javax.swing.LayoutStyle.ComponentPlacement.UNRELATED) 
.addComponent(jButton4, 
javax.swing.GroupLayout.PREFERRED_SIZE, 89, 
javax.swing.GroupLayout.PREFERRED_SIZE)) 
.addComponent(jTextField2, 
javax.swing.GroupLayout.PREFERRED_SIZE, 106, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addComponent(jTextField1, 
javax.swing.GroupLayout.PREFERRED_SIZE, 74, 
javax.swing.GroupLayout.PREFERRED_SIZE)) 
.addContainerGap(569, Short.MAX_VALUE)) 
); 
jPanel1Layout.setVerticalGroup( 
jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(jPanel1Layout.createSequentialGroup() 
.addGap(56, 56, 56) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
BASELINE) 
.addComponent(jLabel1, javax.swing.GroupLayout.PREFERRED_SIZE, 
23, javax.swing.GroupLayout.PREFERRED_SIZE) 
.addComponent(jTextField1, 
javax.swing.GroupLayout.PREFERRED_SIZE, 23, 
javax.swing.GroupLayout.PREFERRED_SIZE)) 
.addGap(33, 33, 33) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
BASELINE) 
.addComponent(jLabel2, javax.swing.GroupLayout.PREFERRED_SIZE, 
26, javax.swing.GroupLayout.PREFERRED_SIZE) 
.addComponent(jTextField2, 
javax.swing.GroupLayout.PREFERRED_SIZE, 26, 
javax.swing.GroupLayout.PREFERRED_SIZE)) 
.addGap(62, 62, 62) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
LEADING, false) 
.addGroup(jPanel1Layout.createParallelGroup(javax.swing.GroupLayout.Alignment.
BASELINE) 
47 
.addComponent(jButton2, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE) 
.addComponent(jButton3, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE) 
.addComponent(jButton4, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)) 
.addComponent(jButton1, javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE)) 
.addContainerGap(362, Short.MAX_VALUE)) 
); 
javax.swing.GroupLayout layout = new 
javax.swing.GroupLayout(getContentPane()); 
getContentPane().setLayout(layout); 
layout.setHorizontalGroup( 
layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(layout.createSequentialGroup() 
.addContainerGap() 
.addComponent(jPanel1, javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, Short.MAX_VALUE) 
.addContainerGap()) 
); 
layout.setVerticalGroup( 
layout.createParallelGroup(javax.swing.GroupLayout.Alignment.LEADING) 
.addGroup(layout.createSequentialGroup() 
.addContainerGap() 
.addComponent(jPanel1, javax.swing.GroupLayout.PREFERRED_SIZE, 
javax.swing.GroupLayout.DEFAULT_SIZE, 
javax.swing.GroupLayout.PREFERRED_SIZE) 
.addContainerGap(42, Short.MAX_VALUE)) 
); 
pack(); 
}// </editor-fold>                         
private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
// TODO add your handling code here: 
try 
{ 
Class.forName("sun.jdbc.odbc.JdbcOdbcDriver"); 
Connection c=DriverManager.getConnection("jdbc:odbc:dsn1"," "," "); 
Statement st=c.createStatement();; 
String s1=jTextField1.getText(); 
int i=Integer.parseInt(s1); 
String s2=jTextField2.getText(); 
48 
49 
 
           int count=st.executeUpdate("insert into student values("+i+",'"+s2+"')"); 
           System.out.println("Record Inserted "+count); 
            } 
        catch(Exception e) 
             { 
                 System.out.println("Insert Exp "+e); 
             } 
    }                                         
    private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here: 
        try 
            { 
           Class.forName("sun.jdbc.odbc.JdbcOdbcDriver"); 
         Connection c=DriverManager.getConnection("jdbc:odbc:dsn1"," "," "); 
           Statement st=c.createStatement();; 
           String s1=jTextField1.getText(); 
           int i=Integer.parseInt(s1); 
           String s2=jTextField2.getText(); 
           int count=st.executeUpdate("update student set sname='"+s2+"' where 
rno="+i+""); 
           System.out.println("Record Updated "+count); 
            } 
        catch(Exception e) 
             { 
                 System.out.println("Update Exp "+e); 
             } 
    }                                         
    private void jButton3ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here: 
        try 
            { 
           Class.forName("sun.jdbc.odbc.JdbcOdbcDriver"); 
         Connection c=DriverManager.getConnection("jdbc:odbc:dsn1"," "," "); 
           Statement st=c.createStatement();; 
           String s1=jTextField1.getText(); 
           int i=Integer.parseInt(s1); 
           int count=st.executeUpdate("delete * from student where rno="+i+""); 
           System.out.println("Record Deleted "+count); 
            } 
        catch(Exception e) 
             { 
                 System.out.println("Delete Exp "+e); 
             } 
    }                                         
    private void jButton4ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here: 
        try 
            { 
Class.forName("sun.jdbc.odbc.JdbcOdbcDriver"); 
Connection c=DriverManager.getConnection("jdbc:odbc:dsn1"," "," "); 
Statement st=c.createStatement();; 
String s1=jTextField1.getText(); 
int i=Integer.parseInt(s1); 
ResultSet rs=st.executeQuery("select * from student where rno="+i+""); 
while(rs.next()) 
{ 
} 
} 
jTextField2.setText(rs.getString("sname")); 
catch(Exception e) 
{ 
System.out.println("Select Exp "+e); 
} 
}                                         
/** 
* @param args the command line arguments 
*/ 
public static void main(String args[]) { 
/* Set the Nimbus look and feel */ 
//<editor-fold defaultstate="collapsed" desc=" Look and feel setting code 
(optional) "> 
/* If Nimbus (introduced in Java SE 6) is not available, stay with the default look 
and feel. 
* For details see 
http://download.oracle.com/javase/tutorial/uiswing/lookandfeel/plaf.html  
*/ 
try { 
for (javax.swing.UIManager.LookAndFeelInfo info : 
javax.swing.UIManager.getInstalledLookAndFeels()) { 
if ("Nimbus".equals(info.getName())) { 
javax.swing.UIManager.setLookAndFeel(info.getClassName()); 
break; 
} 
} 
} catch (ClassNotFoundException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (InstantiationException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (IllegalAccessException ex) { 
50 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} catch (javax.swing.UnsupportedLookAndFeelException ex) { 
java.util.logging.Logger.getLogger(NewJFrame.class.getName()).log(java.util.loggin
g.Level.SEVERE, null, ex); 
} 
//</editor-fold> 
/* Create and display the form */ 
java.awt.EventQueue.invokeLater(new Runnable() { 
public void run() { 
new NewJFrame().setVisible(true); 
} 
}); 
} 
// Variables declaration - do not modify                      
private javax.swing.JButton jButton1; 
private javax.swing.JButton jButton2; 
private javax.swing.JButton jButton3; 
private javax.swing.JButton jButton4; 
private javax.swing.JLabel jLabel1; 
private javax.swing.JLabel jLabel2; 
private javax.swing.JPanel jPanel1; 
private javax.swing.JTextField jTextField1; 
private javax.swing.JTextField jTextField2; 
// End of variables declaration                    
} 
10. Right Click in Code-Run File 
OUTPUT:- 
51 
Assignment 14) Write a program that demonstrates package creation and use in 
program. 
package assignment14; 
import mypackage.NewClass; 
public class Assignment14  
{ 
public static void main(String[] args)  
{ 
NewClass n=new NewClass(); 
n.show(); 
} 
} 
//Create mypackage, Create NewClass 
package mypackage; 
public class NewClass  
{ 
public void show() 
{ 
System.out.println("Show Method is Called"); 
} 
} 
OUTPUT:- 
Show Method is Called 
52 
