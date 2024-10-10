// Java code for linearly searching for x in arr[]. If x
// is present then return its location, otherwise return -1
// Modified by Ruyuf alharbi, ID: 44510064

class LinearSearch {

    // This function returns the index of element x in arr[]
    static int search(int arr[], int n, int x) {

        // Loop through the array to find the element
        for (int i = 0; i < n; i++) {

            // Return the index if the element is found
            if (arr[i] == x)
                return i;
        }

        // Return -1 if the element is not found
        return -1;
    }

    public static void main(String[] args) {

        // Updated the array and search element
        int[] arr = { 3, 4, 1, 7, 5 };
        int n = arr.length;
        int x = 4;  // You can change this value as needed

        // Call the search function
        int index = search(arr, n, x);

        // Output the result
        if (index == -1)
            System.out.println("Element is not present in the array");
        else
            System.out.println("Element found at position " + index);
    }
}
