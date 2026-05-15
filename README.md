# GO2W Racing: How Fast is Your Dog
**Course / Assignment:** [Insert Course Name] Final Report  
**Date:** May 15, 2026  

---

## 1. Introduction

### (a) Project Goal
Fast and stable racing with Go2W in Berkeley Autonomous Racing Car (BARC) track.

### (b) The Challenges
a. Long horizon. In the context of racing, a minimum of 1.5m/s of feedfoward horizon is a must.
b. High dimensionality of joint space for Go2W with highly non-linear system, which makes finite-horizon prediction optimization computationally infeasible.
c. High-speed nature of this task makes domain transfer of RL policy from simulator to reality extremely challenging.

---

## 2. Design

### (a) Design Criteria & Desired Functionality
* **Criteria 1:** Fast, able to finish one lap with average speed of 2.5 m/s
* **Criteria 2:** Stable, able to finish at least 10 laps.

### (b) Chosen Design


### (c) Design Choices and Trade-offs
Our hierarchy design brings together the advantages of both RL and MPPI.
1. RL is good at short-horizon immediate velocity tracking for complex joint dynmaics. At the same time, it provides a compact interface to high-level planner.
2. MPPI uses the compact interface provided by RL to make predictions computationally feasible.

### (d) Impact on Real-World Engineering Criteria
Our experimental result validates the argument that the RL-velocity tracking is never perfect. To enable

---

## 3. Implementation


## 4. Results

### (a) Performance and Tasks Performed
[How well did it work? Be honest! Describe the specific tasks the system successfully completed. If it failed at certain tasks, briefly mention that here too.]

### (b) Visual Results & Video Demonstration
[Embed your main video here. You can upload it to YouTube and link it. Below is the markdown format for a linked video thumbnail, or you can just provide a direct hyperlink.]

[![Watch the video](https://img.youtube.com/vi/YOUR_VIDEO_ID/maxresdefault.jpg)](https://youtu.be/YOUR_VIDEO_ID)
*(Click the image above to watch our project in action!)*

*![Photo of final robot performing task](link-to-photo.jpg)*

---

## 5. Conclusion

### (a) Results Discussion
[Did your finished solution meet the design criteria outlined in Section 2a? Elaborate on the successes.]

### (b) Difficulties Encountered
[What were the biggest roadblocks? Was it hardware integration? A tricky software bug? Tuning a PID controller?]

### (c) Flaws, Hacks, and Future Improvements
[No project is perfect. Did you have to duct-tape a sensor or hardcode a specific value just to get it working for the demo? Own up to it here, and explain how you would do it properly if you had an extra month of development time.]

---

## 6. Team

* **[Yuxiang Liu]**: liu.yx@berkeley.edu
