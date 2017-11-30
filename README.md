# Encryption-Decryption 
public class Cipher
 {
   private String valuetoEncrypt; 
   
   public Cipher (String m)
   {
      valuetoEncrypt = m;
    }
   
   
   public void encryptString() 
   {
      System.out.println("Your string in ASCII is: ");
      for (int n = 0; valuetoEncrypt.length() > n; n++) //n is a counter
      {
          char character = valuetoEncrypt.charAt(n); 
          int ascii = (int) character; 
          System.out.print(ascii); 
        }
      
      System.out.println(""); //ONLY for aesthetics 
      System.out.println("Your encrypted word is: ");
      for (int n = 0; valuetoEncrypt.length() > n; n++)
      {
          char character = valuetoEncrypt.charAt(n); 
          int ascii = (int) character; 
          ascii++;
          char encryptedWord = (char) ascii;
          System.out.print(encryptedWord + ""); 
          
      }
      System.out.println(""); //again, just for aesthetics
   
    }
}
