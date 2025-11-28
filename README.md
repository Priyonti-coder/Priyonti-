# Write a ja program to create a class called BankAccount with instance variable accountNumber and 
balance and static variable bankName and interestRate.Provide static methods toset and  get static   
variables. Create several BankAccount object and print their details along with the static variables.package Static;         
public class BankAccount {

    private int accountNumber;
    
    private double balance;
    
    static private String bankName;
    
    static private double interestRate;
    
    void set_AccountNumber(int accountNumber){
    
        this.accountNumber=accountNumber;
        
    }
    
    int get_AccountNumber(){
    
        return accountNumber;
        
    }
    
    void set_balance(double balance){
    
        this.balance=balance;
        
    }
    
    static void set_bankName(String bankName){
    
        BankAccount.bankName=bankName;
        
    }
    
    static String get_bankName(){
    
        return bankName;
        
    }
    
    static void set_interestRate(double interestRate){
    
        BankAccount.interestRate=interestRate;
        
    }
    
    static double get_interestRate(){
    
        return interestRate;
        
    }
    
    void display(){
    
        System.out.println("accountNumber" + accountNumber);
        
        System.out.println("balance" + balance);
        
        System.out.println("bankName" + BankAccount.bankName);
        
        System.out.println("interestRate" + BankAccount.interestRate);
        
    }
    
    }
    

    package Static;
    
public class Main {

public static void main(String[] args) {

    BankAccount b3 = new BankAccount();
    
    b3.set_AccountNumber(5535);
    
    b3.set_balance(30000.50);
    
    BankAccount.set_bankName("rupaliBank");
    
    BankAccount.set_interestRate(3000.00);
    
    b3.display ();
    
    }
    
}


Output: 

accountNumber5535

balance30000.5

bankNamerupaliBank

interestRate3000.0

BUILD SUCCESSFUL (total time: 0 seconds)

