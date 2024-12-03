# Digital-Forensics

# Digital Forensic Tools Evaluation Project

## Executive Summary

### Objective
Bottom Line Up Front: BLUF: This was a great way for hands on experience. 
This project evaluated digital forensic tools across four forensic analysts, using the NPS Test Disk Images dataset to objectively assess tool accuracy, efficiency, and usability. By simulating a real-world forensic analysis with pre-determined data points, the project sought to identify the capabilities and limitations of various digital forensics tools in identifying, recovering, and analyzing artifacts within a standardized framework.

### Methodology
The project leverages the nps-2009-canon2 dataset from Digital Corpora, which contains images taken with a Canon digital camera. This dataset is ideal for testing basic file recovery, fragmented file recovery, and file carving. Each analyst is assigned specific forensic tools, chosen for their widespread use and unique analytical features:

1. Analyst A: Autopsy and The Sleuth Kit
2. Analyst B: Volatility
3. Analyst C: Magnet RAM Capture
4. Analyst D: CAINE (Computer Aided Investigative Environment) and ExifTool

Each analyst will follow a structured process across all tools:

- Data Acquisition: Import the disk image and verify its hash to ensure data integrity.
- Artifact Analysis: Search for controlled artifacts like deleted files, user activity, and metadata.
- File Recovery: Recover fragmented files and verify findings against known artifacts.
- Documentation: Record tool performance, including detection accuracy, speed, and user interface strengths and limitations.

### Key Findings

1. Accuracy in Artifact Detection:
   - Autopsy and The Sleuth Kit detected deleted files and system logs well, consistently identifying controlled artifacts with high accuracy.
   - Volatility showed strengths in-memory analysis, revealing running processes with detailed accuracy.

2. Efficiency and Speed:
   - Tools with built-in indexing (like Autopsy) provided faster results in artifact detection and keyword searches.
   - ExifTool excelled in handling metadata extraction but required more manual input to achieve optimal results.

3. Usability and Feature Depth:
   - Autopsy was highly user-friendly, with an intuitive interface that reduced analysis time.
   - The Sleuth Kit, while powerful, had a steeper learning curve, requiring more advanced forensic knowledge to yield detailed results.

4. Limitations Identified:
   - Some tools struggled with partial file recovery, such as recovering only fragments of large deleted files.
   - Memory analysis capabilities varied significantly, with Volatility providing deep analysis while other tools offered limited memory forensics features.

## Conclusion

This project highlighted the need to choose the appropriate forensic tool for different investigative tasks. Some tools were best for file recovery and system log analysis, while others excelled in memory forensics and metadata extraction. The controlled dataset allowed objective benchmarking of each tool's performance in terms of data accuracy, recovery speed, and usability.

## Recommendations

1. Tool Selection Based on Task: Tools like Autopsy are recommended for their versatility and accuracy in broad investigations. Volatility (memory analysis) and ExifTool (metadata extraction) are optimal choices for specialized analyses.

2. Continued Testing with Controlled Datasets: Future evaluations should incorporate diverse datasets to assess how these tools perform across operating systems and data types.

3. Training on Complex Tools: To maximize investigative capability, analysts should receive training on complex but powerful tools like The Sleuth Kit.

4. Integration of Tools: Consider workflows integrating multiple tools to leverage their strengths, such as using Autopsy for initial analysis and ExifTool for detailed metadata examination.

5. Regular Tool Updates: Ensure all tools are up-to-date to benefit from the latest features and security patches.

