Signals and Systems (EEL 2010)
Coding Assignment

Description:

This assignment aims to determine the type of filtering applied to an input signal 
 x(t) to produce an output signal 
y(t). The filtering can be categorized into three types: Low Pass, High Pass, or Band Pass. The methodology involves implementing scripts for each filter type, convolving them with the input signal to obtain filtered outputs, and comparing these outputs with the given output signal using correlation.

Methodology:

Filter Design: Three types of filters are designed:
Low Pass Filter (hlp(t)): This filter attenuates high-frequency components and allows low-frequency components to pass.
High Pass Filter (hhp(t)): It attenuates low-frequency components and allows high-frequency components to pass.
Band Pass Filter (hbp(t)): This filter allows a certain range of frequencies (band) to pass while attenuating frequencies outside this range.
Filtering Process:
Each designed filter is convolved with the input signal 
 

x(t) to obtain filtered outputs:
 y lp(t) for Low Pass Filter
 y hp(t) for High Pass Filter
 bp (t) for Band Pass Filter

Correlation Analysis:
The filtered outputs 
 Y lp(t), ℎ y hp(t), and y bp (t) are compared with the given output signal 
y(t) using correlation.
Correlation measures the similarity between two signals. A higher correlation indicates a better match between the filtered output and the given output signal.
Identification of Filter Type:
Based on the correlation results, the filter type that yields the highest correlation with the given output signal is identified.
The identified filter type represents the type of filtering applied to the input signals x(t).
Installation Instructions:-

HERE IS THE CODE AND OUTPUT FILE AND INPUT FILE:-

https://drive.google.com/file/d/1NJxURiNNIxkiMAH4TNhVhwk_w5lalPTD/view?usp=drive_link  -INPUT LINK

https://drive.google.com/drive/folders/1hhBbAwZIXYLt6Ks6E5nhD3HxgeqHyf4E?usp=drive_link -OUTPUT LINK

https://github.com/25dhananjay/SNS-CODING-ASSIGNMENT/blob/main/SNS_codingAssign.ipynb -CODE LINK (GITHUB)

This code performs several signal processing tasks using filters and correlation analysis. Here's a step-by-step explanation:

1. Import Libraries: The code begins by importing the necessary libraries, primarily `matplotlib.pyplot` for plotting.

2. Define Filter Functions: Three filter functions are defined: `low_pass_filter`, `high_pass_filter`, and `band_pass_filter`. Each function implements a different type of filter (low-pass, high-pass, and band-pass) using convolution operations.

3. Define Correlation Function: The code defines a function named `correlation` to calculate the correlation between two signals using numpy's `np.correlate` function.

4. Load Input and Output Signals: The input signal (`input_signal`) and the given output signal (`given_output_signal`) are loaded from external files.

5. Plot Input and Output Signals: Using `matplotlib.pyplot`, the input signal and the given output signal are plotted in separate subplots.

6. Set Filter Parameters: Parameters such as cutoff frequencies and sampling rate are defined for each type of filter.

7. Apply Filters: The input signal is passed through each type of filter: low-pass, high-pass, and band-pass. The filtered signals are stored in `lpf_output`, `hpf_output`, and `bpf_output`, respectively.

8. Calculate Correlation: The correlation between each filtered output signal and the given output signal is calculated using the `correlation` function.

9. Normalize Correlation Values: The correlation values are normalized by dividing each by its maximum value.

10. Print Normalized Correlation Values: The normalized correlation values for each filter type are printed.

11. Calculate Average Normalized Correlation: The average of the normalized correlation values for each filter type is calculated.

12. Print Average Normalized Correlation Values: The average normalized correlation values for each filter type are printed.

13. Determine the Best Filter: Based on the average normalized correlation values, the best filter is determined.

14. Plot Signals and Correlation Values: Using `matplotlib.pyplot`, the input signal, output signals, and normalized correlation values are plotted in separate subplots.

15. Plot the Output of the Best Filter: The output of the best filter is plotted along with the given output signal.

16. Display Plots: All the plots are displayed.

17. Click the github link given above
18. You will able to find the code on screen
19. Copy the code(assignment code) and run this on software  VISUAL CODE  By pasting the code in VS Code.
20. There will be the graph as a result of the CODE

This code essentially processes input signals through different filters and analyzes their correlation with a given output signal to determine the effectiveness of each filter in reproducing the output. Finally, it selects the best filter based on the correlation analysis.

