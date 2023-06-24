/*Input: l1 = [2,4,3], l2 = [5,6,4]
Output: [7,0,8]
Explanation: 342 + 465 = 807.

Input: l1 = [9,9,9,9,9,9,9], l2 = [9,9,9,9]
Output: [8,9,9,9,0,0,0,1]

*/


import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        int len1, len2;
        Scanner input = new Scanner(System.in);
        System.out.print("Enter len : ");
        len1 = input.nextInt();
        System.out.print("Enter len : ");
        len2 = input.nextInt();
        int[] l1 = new int[len1];
        int[] l2 = new int[len2];
        System.out.println("Enter elements of l1: ");
        for (int i = 0; i < len1; i++) {
            l1[i] = input.nextInt();
        }
        System.out.println("Enter elements of l2: ");
        for (int i = 0; i < len2; i++) {
            l2[i] = input.nextInt();
        }
        process(l1, l2);
    }

    static void process(int[] l1, int[] l2) {
        int n1 = l1.length;
        int n2 = l2.length;
        int mi = (n1 > n2) ? n2 : 0;
        int maximum = Math.max(n1, n2);
        int[] res = new int[maximum +1];
        int rem = 0;
 System.out.println(maximum);
        for (int j = 0; j < maximum; j++) {
            int num1 = (j < n1) ? l1[j] : 0;
            int num2 = (j < n2) ? l2[j] : 0;
            int sum = num1 + num2 + rem;
            res[j] = sum % 10;
            rem = sum / 10;
        }
        if (rem != 0) {
            res[maximum] = rem;
           
        }
        System.out.println("Output:");
        for (int i = 0; i<=maximum; i++) {
            System.out.print(res[i] + " ");
        }
    }
}
