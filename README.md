# Bubble Sort Visualizer

A vanilla JavaScript web application that visualizes the Bubble Sort algorithm in real-time.

### The Logic Behind the Algorithm



The "Bubble" sort logic works by repeatedly stepping through the list, comparing adjacent elements and swapping them if they are in the wrong order.

* **Adjacent Comparison**: The inner loop (`j`) compares the current element `array[j]` with the next element `array[j + 1]`.
* **The Swap**: If the element on the left is larger than the one on the right, their values are swapped in the array and their visual heights are updated in the DOM.
* **Bubbling Effect**: With each full pass of the outer loop (`i`), the largest unsorted value "bubbles up" to its correct final position at the end of the array.
* **Optimization**: As the algorithm progresses, the inner loop range decreases (`array.length - i - 1`) because the end of the array becomes increasingly sorted.

### Core Features

* **Real-Time Animation**: Uses `async/await` and a custom `sleep` function to pause execution, allowing users to see each comparison and swap as it happens.
* **Dynamic Array Generation**: Includes a `generateArray` function that clears the previous state and populates the UI with a new set of randomized bars.
* **Visual Feedback**: Implements color-coding where bars turn red during comparison and green once they reach their final sorted position.
* **Interactive Controls**: Features buttons to trigger the sort or reset the data, which automatically disable during the sorting process to prevent logic conflicts.
* **Responsive Styling**: Utilizes a dark-themed CSS layout with Flexbox to ensure bars remain aligned at the bottom of the container regardless of height.

### Technical Stack

* **HTML5**: Semantic structure for the layout and control panel.
* **CSS3**: Flexbox for bar alignment and transitions for smooth color changes.
* **JavaScript**: DOM manipulation and asynchronous logic for the sorting animation.
