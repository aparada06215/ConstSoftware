
import java.util.Scanner;

public class Pendulo
{
    private double longitudCuerda;
    private double aceleracionGravitacional;
    
    public Pendulo (double l, double g){
        this.longitudCuerda=l;
        this.aceleracionGravitacional=g;
    }
    
    public double darlongitudCuerda () {
        return longitudCuerda;
    }
    
    public double darAceleracionGravitacional() {
        return aceleracionGravitacional;
    }
    
    public double periodo () {
        return 2*Math.PI * Math.sqrt (aceleracionGravitacional / longitudCuerda);
    }
    
    public static void main (String[] args) {
        Scanner teclado = new Scanner (System.in);
        
        Pendulo p =null;
        double l,g;
        int opcion = 0;
        
        do {
            System.out.println ("Menu\n1. Crear el pendulo");
            System.out.println ("2. Conocer la longitud de la cuerda");
            System.out.println ("3. Conocer la aceleración gravitacional");
            System.out.println ("4. Conocer el periodo del pendulo");
            System.out.println ("5. salir");
            System.out.print("Ingresa la opción deseada  ");
            opcion = teclado.nextInt();
            
            switch (opcion){
                
                case 1:
                    System.out.print("Ingrese la longitud de la cuerda: ");
                    l= teclado.nextDouble ();
                    System.out.print("Ingrese la aceleración gravitacional: ");
                    g = teclado.nextDouble ();
                    p =  new Pendulo (l,g);
                
                    System.out.println ("Pendulo creado exitosamente");
                break;
                
                case 2:
                    System.out.println ("Longitud de la cuerda = " + p.darlongitudCuerda ());
                break;
                
                case 3:
                    System.out.println ("Aceleración gravitacional = " + p.darAceleracionGravitacional ());
                break;
                
                case 4:
                    System.out.println ("Periodo del Pendulo = " + p.periodo ());
                break;
                
            }
                
            } while (opcion!=5);
            
        System.out.println (" Hemos terminado. ¡Adios!");    
    }
}
