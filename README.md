# Array-Sorting
Sort the array using Javascript

function bubbleSortDescending(arr) {  // 5,3,4,4,9,2
    const n = arr.length;  //6

    for (let i = 0; i < n - 1; i++) {
        for (let j = 0; j < n - i - 1; j++) {
            if (arr[j] < arr[j + 1]) {
                // Swap arr[j] and arr[j + 1]
                const temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }

    return arr;
}

// Example usage
const numbers = [5, 2, 9, 1, 5, 6];
const sortedDescending = bubbleSortDescending(numbers);
console.log(sortedDescending); // Output: [9, 6, 5, 5, 2, 1]

