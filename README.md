# Numberpyramid.java
public class NumberPyramid {
  public static void main(String[] args) {
    int n = 5;
    
   // Outer loop: controls the number of rows (1 to n)
    for(int i = 1; i <= n; i++) {
      
   // Inner loop 1: print spaces for alignment
      // Number of spaces decreases as row number increases
      for(int j = 1; j <= n - i; j++) {
        System.out.print(" ");
      }
      
  // Inner loop 2: print numbers for current row
      // Row i contains numbers from 1 to i
      for(int j = 1; j <= i; j++) {
        System.out.print(j + " ");
      }
      
   // Move to next line after completing each row
      System.out.println();
    }
  }
}
