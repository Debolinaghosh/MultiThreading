# MultiThreading
This Python script demonstrates matrix multiplication with multithreading. It calculates the product of 100 random matrices of size 1000x1000 with a constant matrix of the same size using multiple threads. It also measures the time taken and CPU usage for different numbers of threads.

## Prerequisites
Before running the script, ensure you have the following installed:
- Python 3.x
- NumPy
- psutil (install using `pip install psutil`)
- Matplotlib

# Results:
The script generates two graphs:
- Time Taken vs Number of Threads: This graph shows the time taken for matrix multiplication using different numbers of threads. It also compares the actual time taken with the expected time.
- CPU Usage vs Number of Threads: This graph shows the CPU usage for each CPU core as green grid lines. The peak points are labeled as CPU 0, CPU 1, CPU 2, and so on.

# Conclusion
From the results obtained, we can draw the following conclusions:
- As the number of threads increases, the time taken for matrix multiplication generally decreases, up to a certain point. Beyond that point, the overhead of thread creation and management may outweigh the benefits of parallelism.
- CPU usage increases as the number of threads increases, as expected. However, it's essential to note that the distribution of CPU usage across cores may vary depending on the system architecture and workload.
- It's crucial to optimize the number of threads based on the specific hardware configuration and workload characteristics to achieve the best performance.
- This experiment demonstrates the potential benefits of multithreading for computationally intensive tasks such as matrix multiplication, especially on multicore systems.
