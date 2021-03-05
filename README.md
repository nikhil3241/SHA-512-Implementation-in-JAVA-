# SHA-512-Implementation-in-JAVA-

SHA 512 ENCRYPTION ALGO IN JAVA 
package exercises; 
import java.security.MessageDigest; 
import java.security.NoSuchAlgorithmException; 
public class SHA512String {
          public static void run() { 
                        String myMsg = "Hello World!"; 
                        System.out.println( "Original message: " + myMsg); 
                          try { 
                                  MessageDigest md = MessageDigest.getInstance("SHA-512"); 
                                  byte[] hash = md.digest(myMsg.getBytes()); 
                                  String msgHash = toHexString(hash); 
                                  System.out.println( "Message hash: " + msgHash);
                              } catch(Exception e) { } }
static String toHexString(byte[] array)
{ 
    StringBuilder sb = new StringBuilder(array.length * 2); 
    for (byte b : array) 
        { 
           int value = 0xFF & b;
           // unsigned integer String toAppend = Integer.toHexString(value); 
           sb.append(toAppend).append("-");
        } 
        sb.setLength(sb.length() - 1); 
        return sb.toString().toUpperCase(); 
        } 
}
