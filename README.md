# ARRAYS1D
//Same or not
//SOURCE CODE
import java.io.*;
import java.util.*;
public class Solution {
    public static void main(String[] args) {
        Scanner sc=new Scanner (System.in);
        int n1=sc.nextInt();
        int n2=sc.nextInt();
        int sum1=0,sum2=0;
        int arr1[]=new int[n1];
        int arr2[]=new int[n2];        
        for(int i=0;i<n1;i++){
                arr1[i]=sc.nextInt();  
                sum1+=arr1[i];
            }
        for(int i=0;i<n2;i++){
                arr2[i]=sc.nextInt();
                sum2+=arr2[i];
        }       
        if(n1==n2){            
            if(sum1==sum2){
                System.out.println("Same");
            }
            else{
                System.out.println("Not Same");
            }
        }
        else{
            System.out.println("Not Same");
        }    
      }
}

//Ascending order
//SOURCE CODE
import java.io.*;
import java.util.*;
public class Solution {
    public static void main(String[] args) {
        Scanner sc=new Scanner (System.in);
        int n1=sc.nextInt();
        int arr1[]=new int[n1];
        for(int i=0;i<n1;i++)
        {
            arr1[i]=sc.nextInt();
        }
        System.out.println("The Sorted array is:");
        Arrays.sort(arr1);
        
        for(int i=0;i<n1;i++)
        {
            System.out.println(arr1[i]);
        }
     }
}

//Remove duplicate elements
//SOURCE CODE
import java.io.*;
import java.util.*;
public class Solution {
    public static void main(String[] args) {
        Scanner sc=new Scanner (System.in);
        int a=sc.nextInt();
        int arr[]=new int[a];
        for (int i=0;i<a;i++){
            arr[i]=sc.nextInt();
        }
        for (int i=0;i<a;i++){
            for (int j=i+1;j<a;j++){
                if (arr[i]==arr[j]){
                    arr[j]=-1;
                    
                }
            }
        }
        for (int i=0;i<a;i++){
            if(arr[i]!=-1){
                System.out.println(arr[i]);
            }
        }        
    }
}
