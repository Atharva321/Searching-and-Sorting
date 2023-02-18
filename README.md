# Searching-and-Sorting
# Searching

# Sorting
## Bubble Sort
```
Time : O(n^2)
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
