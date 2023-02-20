# Searching-and-Sorting
# Searching

# Sorting
## Bubble Sort
```
// Time : O(n^2)
public static int[] bubble_sort(int[] a){
        int n = a.length;
        for(int i=0; i<n; i++){
            for(int j=0; j<n-1; j++){
                if(a[j]>a[j+1]){
                    a[j] = a[j]^a[j+1];
                    a[j+1] = a[j]^a[j+1];
                    a[j] = a[j]^a[j+1];
                }
            }
        }
        return a;
}
```
## Selection Sort
```
// Time  : O(n^2)
 public static void selectionSort(int[] arr){  
        for (int i = 0; i < arr.length - 1; i++)  
        {  
            int index = i;  
            for (int j = i + 1; j < arr.length; j++){  
                if (arr[j] < arr[index]){  
                    index = j;//searching for lowest index  
                }  
            }  
            int smallerNumber = arr[index];   
            arr[index] = arr[i];  
            arr[i] = smallerNumber;  
        }  
 }  
```
## Insertion Sort
```
// Time  : O(n^2)
public static void insertionSort(int array[]) {
    int size = array.length;

    for (int step = 1; step < size; step++) {
      int key = array[step];
      int j = step - 1;

      while (j >= 0 && key < array[j]) {
        array[j + 1] = array[j];
        --j;
      }

      array[j + 1] = key;
    }
  }
```
