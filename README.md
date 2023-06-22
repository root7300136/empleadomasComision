# empleadomasComision
comision





public class Empleado {
  private int idEmpleado;
  private String nombreEmpleado;
  private double sueldoBase;
  private double comision;
  
  // Constructor
  public Empleado(int idEmpleado, String nombreEmpleado, double sueldoBase, double comision) {
    this.idEmpleado = idEmpleado;
    this.nombreEmpleado = nombreEmpleado;
    this.sueldoBase = sueldoBase;
    this.comision = comision;
  }
  
  // Getters y setters
  public int getIdEmpleado() {
    return idEmpleado;
  }
  
  public void setIdEmpleado(int idEmpleado) {
    this.idEmpleado = idEmpleado;
  }
  
  public String getNombreEmpleado() {
    return nombreEmpleado;
  }
  
  public void setNombreEmpleado(String nombreEmpleado) {
    this.nombreEmpleado = nombreEmpleado;
  }
  
  public double getSueldoBase() {
    return sueldoBase;
  }
  
  public void setSueldoBase(double sueldoBase) {
    this.sueldoBase = sueldoBase;
  }
  
  public double getComision() {
    return comision;
  }
  
  public void setComision(double comision) {
    this.comision = comision;
  }
  
  // Método para calcular el salario total (sueldo base + comisión)
  public double calcularSalarioTotal() {
    return sueldoBase + comision;
  }






  //Mas salario por comision
  import java.util.Scanner;

public class Main {
  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);
    
    // Obtener los detalles del empleado desde la entrada del usuario
    System.out.println("Ingrese el ID del empleado:");
    int id = sc.nextInt();
    
    System.out.println("Ingrese el nombre del empleado:");
    String nombre = sc.next();
    
    System.out.println("Ingrese el sueldo base del empleado:");
    double sueldoBase = sc.nextDouble();
    
    System.out.println("Ingrese la comisión del empleado:");
    double comision = sc.nextDouble();
    
    // Crear un objeto Empleado con los detalles proporcionados
    Empleado empleado = new Empleado(id, nombre, sueldoBase, comision);
    
    // Calcular el salario total del empleado
    double salarioTotal = empleado.calcularSalarioTotal();
    
    // Imprimir los detalles y el salario total del empleado
    System.out.println("ID: " + empleado.getIdEmpleado());
    System.out.println("Nombre: " + empleado.getNombreEmpleado());
    System.out.println("Sueldo base: " + empleado.getSueldoBase());
    System.out.println("Comisión: " + empleado.getComision());
    System.out.println("Salario total: " + salarioTotal);
  }
}
