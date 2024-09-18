package piedrapapeltijera;

import javax.swing.JOptionPane;

/**
 *
 * @author DisenoDesarrollo
 */
public class java {
 



    public static void main(String[] args) {
        System.out.println("");
        
        /*  entrada        proceso                     salida
            piedra         systema=opcion aleatoria      gano
            papel           entada= opcion              perdio
            tijera                                empate

        */


      String [] opciones = {" piedra","papel","tijera"};
         
      int puntajejugador = 0;  
      int puntajecomputadora = 0;
      int rondas = 3;
      
        for (int i = 0; i < rondas ; i++) { 
            
        }
        int eleccionjugador = JOptionPane.showOptionDialog(null, "seleciona tu jugada","piedra papel o tijera",
                JOptionPane.DEFAULT_OPTION,JOptionPane.INFORMATION_MESSAGE,null,opciones, opciones [0]);
        
      
        
       int eleccioncomputadora = (int)(Math.random()*3);    
        
       
        JOptionPane.showMessageDialog(null, "la computadora eligio :" + opciones[eleccioncomputadora ]);



      if( eleccionjugador == eleccioncomputadora )  {
          JOptionPane.showMessageDialog(null, "empate");
      } else if (( eleccionjugador == 0 && eleccioncomputadora ==2) ||
              ( eleccionjugador == 1 && eleccioncomputadora ==0 )  ||
              (eleccionjugador == 2 && eleccioncomputadora == 1)){
            JOptionPane.showMessageDialog(null, " ganaste esta ronda");
        
      }else{ 
          JOptionPane.showMessageDialog(null, "perdiste esta ronda");
          
      
    
    
      }

    } 
}
