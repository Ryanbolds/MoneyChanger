
import java.util.*;


public class ChangeMachine {
    public static void main(String[] args){
      
          System.out.println("Hello, Welcome to the change ChangeMachine program\n"); 
      
        Scanner dolla = new Scanner(System.in);

       
        System.out.print("Enter an amount from 1 to 99 to make change for: ");
        
        int amount = dolla.nextInt();
        
        int RemainingAmount = (amount);

        int numberOfQuaters = RemainingAmount / 25;  
        RemainingAmount = RemainingAmount % 25;
        
        int numberOfDime = RemainingAmount / 10;  
        RemainingAmount = RemainingAmount % 10;
        
        int numberOfNickel = RemainingAmount / 5;  
        RemainingAmount = RemainingAmount % 5;
        
        int numberOfPenny = RemainingAmount; 
        
        System.out.printf("Coins for %d cents: ", amount);
       if (numberOfQuaters == 1) {
           System.out.printf(" %d quarter, ", numberOfQuaters);}
       else if (numberOfQuaters >= 1){
           System.out.printf(" %d quarters, ", numberOfQuaters); }   
       if (numberOfDime == 1) {
           System.out.printf(" %d dime, ", numberOfDime);}
       else if (numberOfDime >= 1) {
           System.out.printf(" %d dimes, ", numberOfDime);} 
       if (numberOfNickel == 1){
           System.out.printf(" %d nickel, ", numberOfNickel);}
       else if (numberOfNickel >= 1){
           System.out.printf(" %d nickels, ", numberOfNickel);} 
       if (numberOfPenny == 1){
           System.out.printf(" %d penny.", numberOfPenny);}
       else if (numberOfPenny >= 1) {
           System.out.printf(" %d pennies.", numberOfPenny); 
       }
        
  
       System.out.println("\n\nThank you for using ChangeMachine program");
           
       }

    
}
