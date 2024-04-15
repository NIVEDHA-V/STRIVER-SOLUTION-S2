# STRIVER-SOLUTION-S2
## STEP - 2
### SELECTION SORT
The minimum value of the array will be swapped.

```java
public class Solution {
    public static void selectionSort(int[] arr) {
        int temp=0;
        for(int i=0;i<arr.length-1;i++){
            for(int j=i+1;j<arr.length;j++){
                if(arr[i]>arr[j]){
                    temp=arr[i];
                    arr[i]=arr[j];
                    arr[j]=temp;
                }
            }
        }
    }
}
```

### BUBBLE SORT
The maximum value is found and pushed to last by adjacent swapping

```java
public class Solution {
    public static void bubbleSort(int[] arr, int n) {
        int t=0;
        for(int i=n-1;i>=1;i--){
            for(int j=0;j<i;j++){
                if(arr[j]>arr[j+1]){
                    t=arr[j];
                    arr[j]=arr[j+1];
                    arr[j+1]=t;
                }
            }
        }
    }
}
```

### INSERTION SORT
Each element is taken and placed in correct order

```java
public class Solution {
    public static void insertionSort(int[] arr, int size) {
        for(int i=0;i<size;i++){
            int j=i;
            while(j>0&&arr[j-1]>arr[j]){
                int t=arr[j];
                arr[j]=arr[j-1];
                arr[j-1]=t;
                j--;
            }
        }
    }
}
```
