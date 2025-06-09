package flipp_class;

import java.util.Scanner;

public class Maxminvalue {
	    public static void main(String[] args) {
	        Scanner sc = new Scanner(System.in);

	        System.out.print("Size: ");
	        int n = sc.nextInt();
	        int[] a = new int[n];

	        System.out.println("Enter " + n + " numbers:");
	        for (int i = 0; i < n; i++) {
	            a[i] = sc.nextInt();
	        }

	        int min = a[0];
	        int max = a[0];

	        for (int i = 1; i < n; i++) {
	            if (a[i] > max) {
	                max = a[i];
	            }
	            if (a[i] < min) {
	                min = a[i];
	            }
	        }

	        System.out.println("Maximum value: " + max);
	        System.out.println("Minimum value: " + min);

	        sc.close();
	    }
	}
