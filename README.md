# 102103611-Multi-Threading
Methodology :
Matrix Size: Matrices of size NxN are used, where N is chosen to be sufficiently large to ensure a significant computation workload. Constant Matrix: A constant matrix of the same size as the input matrices is generated for multiplication. Thread Configuration: Matrix multiplication is performed using varying numbers of threads, ranging from 1 to 8. Performance Metrics: The time taken to perform matrix multiplication with each thread configuration is measured.

Implementation :
Matrix Generation: Random matrices of the specified size are generated using NumPy. Matrix Multiplication: The matrix multiplication operation is parallelized using Python's threading module. Each thread is responsible for computing a portion of the resulting matrix. Thread Management: Workload is divided among threads to ensure balanced computation. Performance Measurement: The time taken for matrix multiplication with each thread configuration is recorded. Visualization: The results are visualized using matplotlib to show the relationship between the number of threads and the time taken for matrix multiplication.

Results :
![image](https://github.com/Codelord2003/102103058-Multi-Threading/assets/95679005/b2e82bfb-16d1-4560-9961-0988fb8cad6c)

Analysis :

Performance Plateau and Overhead: From  processes 1 onwards, the time taken generally increases with each additional process. This indicates that the overhead of process management, context switching, and communication between processes becomes more significant as the number of processes increases. 

Diminishing Returns: Beyond a certain point  the performance improvement diminishes. In fact, the time taken starts to increase as the number of processes continues to increase. 

System Resource Limitations: The observed behavior could also be influenced by system resource limitations. As the number of processes increases, the system's CPU cores, memory bandwidth, and other resources may become saturated, leading to reduced efficiency and performance.

Graph :
![image](https://github.com/Codelord2003/102103058-Multi-Threading/assets/95679005/15618ff1-f72e-43a1-90b4-bc3f70b8aea8)


![image](https://github.com/Codelord2003/102103058-Multi-Threading/assets/95679005/2f7f485c-1f01-476e-91e8-6e0d8a6a29d9)
![image](https://github.com/Codelord2003/102103058-Multi-Threading/assets/95679005/073c72ba-097e-4640-9767-34082779adc5)
![image](https://github.com/Codelord2003/102103058-Multi-Threading/assets/95679005/63bfc897-2e8b-4d89-98a4-4ad0f6bef110)
![image](https://github.com/Codelord2003/102103058-Multi-Threading/assets/95679005/e01135b3-b711-4627-b828-1c3422a0fb71)



