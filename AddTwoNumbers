
/**
 * Write a description of class addTwoNumbers here.
 * 
 * @author (your name) 
 * @version (a version number or a date)
 */
import java.util.Scanner;

public class AddTwoNumbers
{
    // instance variables - replace the example below with your own
    private String str;
    private int total;

    /**
     * Constructor for objects of class addTwoNumbers
     */
    public AddTwoNumbers()
    {
       total = 0;
       
       Scanner teclado = new Scanner(System.in);
       System.out.print("Ingrese 2 Números entre el 1 y 100 separados por espacio");
       str = teclado.nextLine();
       String[] elementos = str.split("\\s+");
   
       for(int i = 0; i < elementos.length; i++){
           total = total + Integer.parseInt(elementos[i]);
           // System.out.print("elementos" + elementos[i]);
        }
   
       System.out.print("La suma de los " + elementos.length + " números es: " + total);

    }
}
