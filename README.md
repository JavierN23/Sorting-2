Question 1: ![Sorting](https://github.com/user-attachments/assets/9a9c0993-726f-42e3-9175-b0082779b801)

Question 2: 
#include <iostream>
using namespace std;

void insertionSort(int A[], int n) {
    int steps = 0;

    for (int i = 1; i < n; i++) {
        int key = A[i];
        int j = i - 1;
        
    while (j >= 0 && A[j] > key) {
            A[j + 1] = A[j]; 
            j--;
            steps++;  
        }
        
        A[j + 1] = key;  
        steps++; 
    }

    cout << "Total steps: " << steps << endl; 
}

int main() {
    int A[] = {5, 4, 3, 2, 1};
    int n = sizeof(A) / sizeof(A[0]);  
    insertionSort(A, n);  
    
    cout << "Sorted Array: ";
    for (int i = 0; i < n; i++) {
        cout << A[i] << " ";
    }
    cout << endl;

    return 0;
}

Question 3: What is this function’s time complexity regarding Big O Notation?
The Time Complexity regarding Big O Notation is O(N). This is because the time it takes to run is linear with the string lengths. If the string is larger, the execution time will be longer. Making it linear, resulting in the time complexity O(N).

Question 4: 
function containsX(string) {
    for (let i = 0; i < string.length; i++) {
        if (string[i] === "X") {
            return true;
        }
    }
    return false;
}
Video: https://www.youtube.com/watch?v=23APz7lw-Sw
