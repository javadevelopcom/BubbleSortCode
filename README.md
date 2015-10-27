# BubbleSort
import java.util.Arrays;

public class BubbleSortCode {

    public static void main(String[] args) {

        int[] arr = {20, 15, 1, 68, 2, 35, 77};
        int n = arr.length;
        System.out.println("Unsorted array: " + Arrays.toString(arr));
        for (int k = 0; k < n - 1; k++) {
            for (int i = 0; i < n - k - 1; i++) {
                if (arr[i] > arr[i + 1]) {
                    int temp = arr[i];
                    arr[i] = arr[i + 1];
                    arr[i + 1] = temp;
                }
            }
        }
        System.out.println("Sorted array:   " + Arrays.toString(arr));
    }
}
