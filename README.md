# OS Disk Scheduling Algorithm Simulator

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/JGovardhan2007/adaf6e1f41cf14039ef333e80f54fd33)

An interactive, browser-based simulator built for an **Operating Systems** course project. This application utilizes Google Colab, `ipywidgets`, and Matplotlib to visualize how different disk scheduling algorithms handle an I/O request queue, charting the disk head's path and calculating the **Total Head Movement (Cylinder Seek Distance)** dynamically.

## 🚀 Features

- **Interactive UI Panel:** Easily adjust disk capacity, change the starting head pointer position, and supply custom comma-separated request queues using sliders and input forms right inside the notebook.
- **6 Supported Core Algorithms:**
  - **FCFS** (First-Come, First-Served)
  - **SSTF** (Shortest Seek Time First)
  - **SCAN** (Elevator Algorithm)
  - **C-SCAN** (Circular SCAN)
  - **LOOK**
  - **C-LOOK** (Circular LOOK)
- **Inline Video Animations:** Watch the disk arm travel sequentially frame-by-frame across charts mapped directly through Matplotlib HTML5 video rendering.

## 🛠️ How to Run the Application

You do not need to install anything on your local computer to run this project!

1. Click the **Open In Colab** badge at the top of this README.
2. Once the notebook opens in Google Colab, click the **Connect** button in the top right corner.
3. Click the **Play** button on the code cell to execute the application. (It will automatically verify and load your environment requirements).
4. The **Disk Scheduler Configuration Panel** will appear directly below the cell output.

## 📊 How to Use It

1. Enter the total number of cylinders under **Disk Size** (e.g., `200`).
2. Input the initial location of the disk arm pointer under **Starting Head Position** (e.g., `53`).
3. Supply a track reference chain in the **Request Queue** text block as comma-separated integers (e.g., `98, 183, 37, 122, 14, 124, 65, 67`).
4. Select which algorithm you want to evaluate from the dropdown menu.
5. Click **Generate Animation 🎬**.
6. Wait a few seconds for the calculations to complete, and an interactive video player will embed itself on the page showing the sequential path of the disk head.
