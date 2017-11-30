# Encryption-Decryption

Public class Decipher 
{
   private String valuetoDecrypt; 
   
   public Decipher (String x)
   {
      valuetoDecrypt = x;
    }
   
   public void decryptString()
   { 
     System.out.print("We decrypted your word: ");
       for (int n = 0; valuetoDecrypt.length() > n; n++)
     {
         char everyCharacter = valuetoDecrypt.charAt(n); 
         int asciiValue = (int) everyCharacter -1; 
         char decryptedWord =(char) asciiValue;
         System.out.print(decryptedWord); 
         
       }
     System.out.println(""); 
   }
} 
