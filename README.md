# SETI LAB

band_scan.c is the original unoptimized file.

p_band_scan.c is the optimized file.  Speeds were about 9x as fast.

The p_band_scan.c program implements a parallelized solution for scanning radio frequency signals to detect potential extraterrestrial communication, designed as part of the Northwestern CS 213 SETI Lab. By leveraging Pthreads, the program divides the workload of processing multiple frequency bands across multiple threads, significantly reducing runtime compared to the sequential implementation. Users can customize the execution by specifying the number of threads and processors to optimize performance. The program applies band-pass filters to isolate power within each frequency band and identifies high-power signals in the range of interest (50 kHz - 150 kHz) as potential alien transmissions, marking them with a (WOW) in the output. Techniques such as processor affinity and convolution-based filtering are used to maximize efficiency and scalability. The program also measures execution time and resource usage to aid in performance tuning. This project emphasizes the application of low-level parallel programming techniques to optimize computationally intensive tasks.
