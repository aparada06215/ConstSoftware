import java.util.Scanner;
import java.util.ArrayList;
// crear clase empleado
public class Empleado
{
    private String nombre;
    private String departamento;
    private String posicion;
    private int salario;

    //Los cuatro metodos siguientes retornan cada atributo del objeto Empleado
    public String getNombre(){
        return nombre;
    }

    public String getDepartamento(){
        return departamento;
    }

    public String getPosicion(){
        return posicion;
    }

    public int getSalario(){
        return salario;
    }

    //metodo para imprimir la información del empleado en pantalla
    public void imprimir (ArrayList<Empleado>  empleados) {
        System.out.println("----------------------------------LISTADO-------------------------------------------");
        //En este for se itera el ArrayList donde se almacenó cada instancia del objeto Empleado
            for (int i = 0; i < empleados.size(); i++) {
            System.out.print(+(i+1)+". Nombre: " + empleados.get(i).getNombre());
            System.out.print(" | Departamento: " + empleados.get(i).getDepartamento());
            System.out.print(" | Posición: " + empleados.get(i).getPosicion());
            System.out.println(" | Salario: " + empleados.get(i).getSalario());
            System.out.println("--------------------------------------------------------------------------------");
        }  
    }

    //Metodo asignar nombre al empleado
    public void asignarNombre (String nuevoNombre) {
        nombre = nuevoNombre;
    }

    //Metodo asignar departamento al empleado
    public void asignarDepartamento (String nuevoDepartamento) {
        departamento = nuevoDepartamento;
    }

    //Metodo asignar posición al empleado
    public void asignarPosicion (String nuevaPosicion) {
        posicion = nuevaPosicion;
    }

    //Metodo asignar salario al empleado
    public void asignarSalario (int nuevoSalario) {
        salario = nuevoSalario;
    }

    //Programa principal
    public static void main (String [] args) {
        Scanner teclado = new Scanner(System.in);
        ArrayList <Empleado> empleados = new ArrayList <Empleado> ();//lista de empleados
        int opc = 0;
        String nom, dep, pos, pre;
        int sal;
        Empleado e = null;
        //e=new Empleado();
        do {
            System.out.println("Supermercado Santa Fe");
            System.out.println("Menu");
            System.out.println("1. Agregar nuevo empleado");
            System.out.println("2. Asignar Nombre al empleado");
            System.out.println("3. Asignar Departamento al empleado");
            System.out.println("4. Asignar Posición al empleado");
            System.out.println("5. Asignar Salario al empleado");
            System.out.println("6. Conocer lista de empleados");
            System.out.println("7. Salir");
            System.out.println("Ingrese una opción");
            opc = teclado.nextInt();
            
            switch (opc) {
                //Este case crea una nueva instancia del objeto Empleado, por lo que al registrar la información otra vez, ya sería un empleado nuevo
                case 1:
                e = new Empleado();
                System.out.println("---------------------------------Empleado creado-----------------------------");
                System.out.println("Ingrese a la opción 2 para agregar el nombre del empleado");
                System.out.println("-----------------------------------------------------------------------------");
                empleados.add(e);
                break;

                case 2:
                System.out.println("-----------------------------------------------------------------------------");
                System.out.print("Ingrese nombre del empleado: ");
                teclado.nextLine();
                nom = teclado.nextLine();                
                e.asignarNombre(nom);
                System.out.println("-----------------------------------------------------------------------------");
                break;

                case 3:
                System.out.println("-----------------------------------------------------------------------------");
                System.out.print("Departamento al que pertenece el empleado: ");
                teclado.nextLine();
                dep = teclado.nextLine();                
                e.asignarDepartamento(dep);
                System.out.println("Departamento asignado");
                System.out.println("-----------------------------------------------------------------------------");
                break;

                case 4:
                System.out.println("-----------------------------------------------------------------------------");
                System.out.print("Posición del empleado: ");
                teclado.nextLine();
                pos = teclado.nextLine();
                e.asignarPosicion(pos);
                System.out.println("Posición asignada");
                System.out.println("-----------------------------------------------------------------------------");
                break;

                case 5:
                System.out.println("-----------------------------------------------------------------------------");
                System.out.print("Salario del empleado: ");
                teclado.nextLine();
                sal = teclado.nextInt();                
                e.asignarSalario(sal);
                System.out.println("Salario asignado");
                System.out.println("-----------------------------------------------------------------------------");
                break;
                   
                case 6:
                System.out.println("-----------------------------------------------------------------------------");
                if (empleados == null || empleados.size()==0){
                   System.out.println("No existen empleados en la lista");
                }
                else {
                    e.imprimir(empleados);
                }
                break;
            }
        }while (opc !=7);
        System.out.println (" Hemos terminado. ¡Adios!"); 
    }
}
