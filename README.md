/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package com.mycompany.class1;

import javax.swing.JOptionPane;
/**
 *
 * @author Aleja Valbuena
 */
public class JavaParcial1elec {
        public static void main(String[] args) {
            //Se declara las variables
            int numberone=0, numbertwo=0, operation=0;
            //Se monta las variables de int a string
            numberone = Integer.parseInt(JOptionPane.showInputDialog(" por favor ingrese el primer número"));

            numbertwo = Integer.parseInt(JOptionPane.showInputDialog(" por favor ingrese el segundo número"));

            operation = Integer.parseInt(JOptionPane.showInputDialog(" ¿Que tipo de operacion desea hacer?: 1.suma  2.resta  3.multiplicacion  4.division"));

        //Condicion de las operaciones cuando numero 1 es mayor o igual a numero 2
        if (numberone >= numbertwo) {

            if (operation == 1) {
                int suma= numberone+numbertwo;
                JOptionPane.showMessageDialog(null, "Se suma "+ numberone +" + "+ numbertwo + " siendo el resultado de la suma es: "+ suma);
                //Este ciclo coje el resultado y hace su tabla respectiva
                for ( int i = 0; i < 10; i++) {
                    JOptionPane.showMessageDialog(null, +suma +" x " +(i+1) +" = " +(suma * (i+1)));
                }
            }
             if (operation == 2) {
                int resta= numberone-numbertwo;
                JOptionPane.showMessageDialog(null, "Se resta "+ numberone +" - "+ numbertwo + " siendo el resultado de la resta es: "+ resta);
                for ( int i = 0; i < 10; i++) {
                    JOptionPane.showMessageDialog(null, +resta +" x " +(i+1) +" = " +(resta * (i+1)));
                }
            }
              if (operation == 3) {
                int multiplicacion= numberone*numbertwo;
                JOptionPane.showMessageDialog(null, "Se multiplica "+ numberone +" * "+ numbertwo + " siendo el resultado de la multiplicacion es: "+ multiplicacion);
                for ( int i = 0; i < 10; i++) {
                    JOptionPane.showMessageDialog(null, +multiplicacion +" x " +(i+1) +" = " +(multiplicacion * (i+1)));
                }
            }
               if (operation == 4) {
                   if ( numbertwo == 0) {
                       JOptionPane.showMessageDialog(null, "No es posible dividir entre cero");
                   }else {
                int division= numberone/numbertwo;
                JOptionPane.showMessageDialog(null, "Se divide "+ numberone +" / "+ numbertwo + " siendo el resultado de la division es: "+ division);
                for ( int i = 0; i < 10; i++) {
                    JOptionPane.showMessageDialog(null, +division +" x " +(i+1) +" = " +(division * (i+1)));
                }
                }
            }
        //Condicion de las operaciones cuando numero 2 es mayor   
        }else {
            if (operation == 1) {
                int suma= numbertwo+numberone;
                JOptionPane.showMessageDialog(null, "Se suma "+ numbertwo +" + "+ numberone + " el resultado es: "+ suma);
                for ( int i = 0; i < 10; i++) {
                    JOptionPane.showMessageDialog(null, +suma +" x " +(i+1) +" = " +(suma * (i+1)));
                }
            }
             if (operation == 2) {
                int resta= numbertwo-numberone;
                JOptionPane.showMessageDialog(null, "Se resta "+ numbertwo +" - "+ numberone + " siendo el resultado de la resta es: "+ resta);
                for ( int i = 0; i < 10; i++) {
                    JOptionPane.showMessageDialog(null, +resta +" x " +(i+1) +" = " +(resta * (i+1)));
                }
            }
              if (operation == 3) {
                int multiplicacion= numbertwo*numberone;
                JOptionPane.showMessageDialog(null, "Se multiplica "+ numbertwo +" * "+ numberone + " siendo el resultado de la multiplicacion es: "+ multiplicacion);
                for ( int i = 0; i < 10; i++) {
                    JOptionPane.showMessageDialog(null, +multiplicacion +" x " +(i+1) +" = " +(multiplicacion * (i+1)));
                }
            }
               if (operation == 4) {
                   if (numberone == 0) {
                       JOptionPane.showMessageDialog(null, "No es posible dividir entre cero");
                int division= numbertwo/numberone;
                JOptionPane.showMessageDialog(null, "Se divide "+ numbertwo +" / "+ numberone + " siendo el resultado de la division es: "+ division);
                for ( int i = 0; i < 10; i++) {
                    JOptionPane.showMessageDialog(null, +division +" x " +(i+1) +" = " +(division * (i+1)));
                }
                }
            }

        }

    }  
}
