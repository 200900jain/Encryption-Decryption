# Encryption-Decryption
public class ImitationGame
{
    public static void main(String[] args) 
    {
        Cipher computer = new Cipher("hello"); 
        computer.encryptString();
        
        Decipher science = new Decipher("ifmmp");
        science.decryptString();
    }
}
