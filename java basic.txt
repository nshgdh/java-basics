28-04-2025

1.TO PRINT N NUMBERS 

import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        for(int i = 1;I<=1;i++){
            System.out.print(i);
        }

        
    }
}

2.TO PRINT N NUMBERS IN REVERSE


import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        for(int i = n;i>=1;i--){
            System.out.print(i);
        }

        
    }
}

3.TO PRINT N NUMBERS IN REVERSING USING RECURSION


import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        printnos(n);
    }

    public static void printnos(int n){
        if (n == 0) {
            return;
        }
        System.out.print(n + " ");
        printnos(n - 1);
    }
}

4.TO PRINT N NUMBERS USING RECUSION 

import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        printnos(n);  // Start from 1
    }

    public static void printnos( int n) {
        if ( n==0) {
            return;
        }
             printnos(n-1);
	System.out.print(n); 
       
    }
}

5. FACTORIAL PROGRAM

import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int fact = 1;
        for(int i = 1; i <= n; i++){ 
             fact = fact * i; 
        }
        System.out.println(fact);
    }
}


6.FACTORIAL USING RECURSION 

import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in); 
        int n = sc.nextInt();
        
        int result = Factorial(n); 
        System.out.println(result); 
    }

    public static int Factorial(int n) {
        if (n == 0 || n == 1) { 
            return 1;
        } else { 
            return n * Factorial(n - 1);
        }
    }
}

7.SUM OF N NATURAL NUMBERS

import java.util.*;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in); 
        int n = sc.nextInt();
        
        int result = SumOf(n); 
        System.out.println(result); 
    }

    public static int SumOf(int n) {
        if (n == 0 )  return 0;
         return n + SumOf(n - 1);
        }
    }

 29-04-2025

8.MAXIMUM ELEMENT IN ARRAY


imfor(int i = 1;i<n;i++){
            System.out.println(arr[i]);}

9.MIMINUM ELEMENT OF ARRAY 


import java.util.*;

public class Main {
    public static void main(String[] args) {
      //  int arr[] = {20,50,40,50,699};
        Scanner sc = new Scanner(System.in); 
        int n = sc.nextInt();
        int []arr = new int[n];
        
        for(int i = 0;i<n;i++){
            arr[i] = sc.nextInt();
        }
        
        int min = arr[0];
for(int i = 0;i<n;i++){
            if(arr[i]<min){
                min = arr[i];
            }
        }
        System.out.println(min);
    }

    
    }

10.TO PRINT HOW MANY ODD NUMBER AND EVEN NUMBER IN A ARRAY


import java.util.*;

public class Main {
    public static void main(String[] args) {
      //  int arr[] = {20,50,40,50,699};
        Scanner sc = new Scanner(System.in); 
        int n = sc.nextInt();
        int []arr = new int[n];
        
        for(int i = 0;i<n;i++){
            arr[i] = sc.nextInt();
            
        }
        int even = 0;
            int odd = 0;
        for(int i = 0; i<n; i++){
        if(arr[i]%2==0){
             even++;
            }
            else{
                odd++;
            }}
       System.out.println(even);
       System.out.println(odd);
    }


    
    }

11.TO SUM THE ELEMENT IN ARRAY


import java.util.*;

public class Main {
    public static void main(String[] args) {
      
        Scanner sc = new Scanner(System.in); 
        int n = sc.nextInt();
        int []arr = new int[n];
        
        for(int i = 0;i<n;i++){
            arr[i] = sc.nextInt();
            
        }
         int sum=0;
        for(int i = 0; i<n; i++){
        sum +=arr[i];
            }
       System.out.println(sum);
       
    }}


    
    
12.TO FIND THE AVERAGE OF ARRAY


import java.util.*;

public class Main {
    public static void main(String[] args) {
      
        Scanner sc = new Scanner(System.in); 
        int n = sc.nextInt();
        int []arr = new int[n];
        
        for(int i = 0;i<n;i++){
            arr[i] = sc.nextInt();
            
        }
         int sum=0;
        for(int i = 0; i<n; i++){
        sum +=arr[i];
            }
       System.out.println(sum);
       int avg = 1;
       for(int i = 0;i<n;i++){
         avg = (sum/n);
       }
       System.out.println(avg);
    }}


    
    
13. TO ADD ELEMENTS FROM RIGHTSIDE AND STORE IT IN LEFT SIDE


import java.util.*;

public class Main {
    public static void main(String[] args) {
      
        Scanner sc = new Scanner(System.in); 
        int n = sc.nextInt();
        int []arr = new int[n];
        
        for(int i = 0;i<n;i++){
            arr[i] = sc.nextInt();
            
        }
         int sum=0;
        for(int i = arr.length-1; i>=0; i--){
        int temp = arr[i];
        arr[i] = sum;
        sum = sum+temp;}
        for(int i = 0;i<arr.length;i++){
            System.out.print(arr[i]+" ");
        }
    }}

14.TO ADD ELEMENTS FROM LEFT TO RIGHT AND STORE IN RIGHT SIDE



import java.util.*;

public class Main {
    public static void main(String[] args) {
      
        Scanner sc = new Scanner(System.in); 
        int n = sc.nextInt();
        int []arr = new int[n];
        
        for(int i = 0;i<n;i++){
            arr[i] = sc.nextInt();
            
        }
         int sum=0;
         for(int i = 0;i<arr.length;i++) {
        int temp = arr[i];
        arr[i] = sum;
        sum = sum+temp;}
        for(int i = 0; i<=arr.length-1; i++)
       {
            System.out.print(arr[i]+" ");
        }
    }}


 30-04-2025 
    
15.INPUT : {1 2 3 4 5 6 7 8 9 10}
   OUTPUT : {5 6 7 8 9 10 1 2 3 4}
   TARGET : 4

import java.util.*;

public class Main {
    public static void main(String[] args) {
        
        Scanner sc = new Scanner(System.in);

       
        int n = 10;
        int[] arr = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};  
        int k = 5;  

        
        k = k % n;

        
        for (int i = 0; i < n / 2; i++) {
            int temp = arr[i];
            arr[i] = arr[n - i - 1];
            arr[n - i - 1] = temp;
        }


        for (int i = 0; i < k / 2; i++) {
            int temp = arr[i];
            arr[i] = arr[k - i - 1];
            arr[k - i - 1] = temp;
        }

        
        for (int i = k; i < (n + k) / 2; i++) {
            int temp = arr[i];
            arr[i] = arr[n - i + k - 1];
            arr[n - i + k - 1] = temp;
        }

        
        System.out.println();
        for (int i = 0; i < n; i++) {
            System.out.print(arr[i] + " ");
        }

        sc.close();
    }
}


16.TO SUM THE ERROR USING SLIDING

import java.util.*;

public class Main {
    public static void main(String[] args) {
        
        int[] arr = {1,2,3,4,5};

        int ws = 0; 
        int k = 2;  
        int c = 0;  
        double avg = 1;
        
       
        for (int i = 0; i < k; i++) {
            ws = ws + arr[i];
        }
        c++; 

        
        for (int i = k; i < arr.length; i++) {
            
            ws = ws - arr[i - k] + arr[i];
            c++;
        }if(c!=0){
             avg = ws/5;
        }

        System.out.println( c);
        System.out.print(avg);
    }
}


 05-05-2025

17. TO PRINT 2D ARRAY

import java.util.*;
public class Main{
    public static void main(String[] args){
        int[][] arr = {{1,2,3},{4,5,6},{7,8,9}};
        for(int i =0;i<arr.length;i++){
           for(int j =0;j<arr[i].length;j++){
            System.out.print(arr[i][j]+" ");
        }
    System.out.println();
    }
    }
}


18. TO PRINT 2D ARRAY FROM USER INPUT

import java.util.*;
public class Main{
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        int[][] arr = new int[a][b];
        for(int i =0;i<a;i++){
            for(int j =0;j<b;j++){
            arr[i][j] = sc.nextInt();
         }}
        for(int i =0;i<a;i++){
           for(int j =0;j<b;j++){
            System.out.print(arr[i][j]+" ");
        }
    System.out.println();
    }
    }
}

19.  TO ADD ALL THE ELEMNETS IN THE ARRAY

import java.util.*;
public class Main{
    public static void main(String[] args){
       Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        int sum = 0;
        int[][] arr = new int[a][b];
        for(int i =0;i<a;i++)
        {
            for(int j =0;j<b;j++)
            {
            arr[i][j] = sc.nextInt();
             }
        }
        for(int i =0;i<a;i++)
        {
           for(int j =0;j<b;j++)
           {
            sum += arr[i][j];    
           }
    }
    System.out.print(sum);
   
    }
    }

20. TRANSPOSE OF 2D ARRAY

import java.util.*;
public class Main{
    public static void main(String[] args){
       Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        int[][] arr = new int[a][b];
        int[][] temp = new int[b][a];
        for(int i =0;i<a;i++)
        {
            for(int j =0;j<b;j++)
            {
            arr[i][j] = sc.nextInt();
             }
        }
        for(int i =0;i<a;i++)
        {
           for(int j =0;j<b;j++)
           {
             System.out.print(arr[i][j]+" ");    
           }
           System.out.println();
    }
    for(int i =0;i<b;i++)
        {
           for(int j =0;j<a;j++)
           {
             System.out.print(arr[j][i]+" ");    
           }
           System.out.println();
    }
    
   
    }
    }


21. TO PRINT DIAGONAL VALUE IN 2D ARRAY

import java.util.*;
public class Main{
    public static void main(String[] args){
       Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        int[][] arr = new int[a][b];
        int sumrow = 0;
        int sumcol = 0;
       
        for(int i =0;i<a;i++)
        {
            for(int j =0;j<b;j++)
            {
            arr[i][j] = sc.nextInt();
             }
        }
        for(int i =0;i<a;i++)
        { 
           for(int j =0;j<b;j++)
           {
             System.out.print(arr[i][j]+" ");    
           }
           System.out.println();
    } 
    for(int i =0;i<a;i++)
        { 
           for(int j =0;j<b;j++)
           {
             if(i==j) {
                System.out.println(arr[i][j]);
             }   
           }
          
    } 
        }
    }





 

