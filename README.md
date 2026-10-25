# 📊 Sorting Algorithm Visualizer

A Python-based application that visualizes sorting algorithms through animated bar charts. Watch how elements move and change at each step to understand how different sorting algorithms work.

## ✨ Features

- 📈 **Real-Time Visualization** — Watch sorting algorithms operate through animated bar charts.
- 🔀 **Random Array Generation** — Generate random unsorted arrays of a user-defined size.
- 🎯 **Multiple Algorithms** — Choose from five popular sorting algorithms.
- 🎞️ **Smooth Animations** — Visualize intermediate sorting states using Matplotlib.
- ⚙️ **Python Generators** — Use `yield` to expose intermediate states of the sorting process.
- 🧩 **Modular Design** — Keep algorithm implementations, visualization, and program execution in separate files.

## 🛠️ Technologies Used

- **Python 3.x**
- **Matplotlib** — Bar charts and animations
- **Random Module** — Random array generation
- **Generators (`yield`)** — Step-by-step algorithm visualization
- **FuncAnimation** — Updating the chart during animation

## 🧮 Algorithms Implemented

| Algorithm | Best Case | Average Case | Worst Case | Auxiliary Space |
|---|---|---|---|---|
| Bubble Sort | O(n)* | O(n²) | O(n²) | O(1) |
| Selection Sort | O(n²) | O(n²) | O(n²) | O(1) |
| Insertion Sort | O(n) | O(n²) | O(n²) | O(1) |
| Merge Sort | O(n log n) | O(n log n) | O(n log n) | O(n) |
| Quick Sort | O(n log n) | O(n log n) | O(n²) | O(log n)* |

*Complexities depend on implementation. Bubble Sort has O(n) best-case time when optimized with an early-exit check. Quick Sort's auxiliary space is typically O(log n) on average but can reach O(n) in the worst case due to recursion.*

## 📁 Project Structure

```text
Sorting-Algorithm-Visualizer/
├── algorithms.py       # Sorting algorithm implementations
├── vizualizer.py       # Matplotlib visualization and animation
├── main.py             # Main program and user interaction
└── README.md            # Project documentation
```

## 🚀 Getting Started

### Prerequisites

- Python 3.x
- pip package manager

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/Sorting-Algorithm-Visualizer.git
cd Sorting-Algorithm-Visualizer
```

Replace `YOUR_USERNAME` with your GitHub username.

### 2. Install Dependencies

```bash
pip install matplotlib
```

### 3. Run the Application

```bash
python main.py
```

## 🖥️ How to Use

1. Run the application.
2. Enter the desired array size when prompted.
3. Select a sorting algorithm from the menu.
4. Watch the animated bar chart as the algorithm sorts the array.

### Available Algorithms

```text
1. Bubble Sort
2. Selection Sort
3. Insertion Sort
4. Merge Sort
5. Quick Sort
```

## ⚙️ How It Works

The application separates sorting logic from visualization.

1. **Array Generation:** A random unsorted array is generated based on the requested size.
2. **Algorithm Selection:** The user chooses a sorting algorithm.
3. **Step-by-Step Execution:** Sorting algorithms use Python generators to yield intermediate array states.
4. **Animation:** Matplotlib's `FuncAnimation` consumes the yielded states and updates the bar heights.
5. **Visualization:** The animated chart displays the array's progression toward sorted order.

### Example: Python Generators

Instead of returning only the final sorted array, a generator can yield intermediate states:

```python
yield a
```

Each yielded state can be used by the visualization to display the next step in the sorting process.

## 🎯 Learning Objectives

This project demonstrates:

- Sorting algorithm implementation and comparison
- Time and space complexity analysis
- Python generators and the `yield` keyword
- Data visualization using Matplotlib
- Animation with `FuncAnimation`
- Modular programming and separation of concerns

## 🔮 Future Improvements

- Adjustable animation speed
- Pause and resume controls
- Color-coded comparisons, swaps, and sorted elements
- Additional algorithms, including Heap Sort, Counting Sort, and Radix Sort
- Side-by-side comparison of sorting algorithms
- GUI support using Tkinter or PyQt
- Real-time statistics for comparisons and swaps

## 👨‍💻 Author

**Dev Kumar**

- GitHub: [YOUR_USERNAME](https://github.com/YOUR_USERNAME)
- LinkedIn: [Dev Kumar](https://www.linkedin.com/in/dev-kumar-0578402aa)

---

⭐ If you find this project useful, consider giving the repository a star.
