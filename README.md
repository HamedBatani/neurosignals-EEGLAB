# Neurosignals with EEGLAB

This project was part of my *Signals and Systems* course at Sharif University of Technology in Spring 2025, under Professor Hamid Karbalaei Aghajan. I worked on EEG data using MATLAB and EEGLAB, aiming to apply theoretical signal processing concepts to real brain signals.

The project is split into two phases. In the first, I focused on exploring the raw EEG signals and understanding their frequency components. In the second, I used segments of these signals as inputs to modeled systems to explore how the brain’s activity could be processed like a signal in an LTI system.

---


![](https://github.com/HamedBatani/neurosignals-EEGLAB/raw/main/Screenshot%202025-07-30%20091115.png)


## Phase 1 — Analyzing and Filtering EEG Signals

I started by loading EEG data (the `eeglab_data.set` sample dataset) into EEGLAB and selecting channels like `Pz` and `Oz` for analysis. After removing the DC offset, I calculated the energy, power, and RMS of the signal and then applied FFT to inspect its frequency content.

This helped me identify key frequency bands like Alpha (8–13 Hz), Beta (13–30 Hz), and Delta (<4 Hz). I then designed and implemented FIR and Butterworth filters to isolate these bands. Comparing filtered vs. raw signals really highlighted how different brain wave components could be separated and studied individually.

Seeing textbook filters actually clean up noisy EEG signals gave me a clearer understanding of why frequency analysis matters—especially when dealing with biological signals that are inherently messy.
![](https://github.com/HamedBatani/neurosignals-EEGLAB/raw/main/Screenshot%202025-07-30%20091103.png)
---

## Phase 2 — Modeling EEG Signal Flow as an LTI System

In the second phase, I moved away from just analyzing signals to treating them as inputs to systems. I defined a few artificial impulse responses—things like simple exponentials or Gaussian-like curves—and used them to simulate basic LTI systems.

Using convolution, I applied these systems to Alpha-band EEG segments and studied the output. This was a way to explore how different system characteristics (like memory or smoothing) would affect the signal. It also gave me hands-on experience with concepts like impulse response and system behavior in the time domain—outside of the classroom setting.

While the systems weren’t biologically accurate, the process helped me imagine how parts of the brain might process signals differently, or how a device might interpret EEG activity.

---

## What I Used

- MATLAB for processing and visualization  
- EEGLAB toolbox to handle EEG data  
- FFT for frequency analysis  
- FIR and Butterworth filters  
- Convolution with impulse responses to simulate system behavior

---

![](https://github.com/HamedBatani/neurosignals-EEGLAB/raw/main/Screenshot%202025-07-30%20090930.png)
![](https://github.com/HamedBatani/neurosignals-EEGLAB/raw/main/Screenshot%202025-07-30%20091022.png)

---

## Why I Think This Project Is Important

EEG data is real, raw, and often unpredictable. It’s not the clean kind of signal we usually deal with in theoretical coursework. But that’s exactly why I found this project valuable: it forced me to apply what I learned to something complex and messy—and make sense of it.

Working with EEG signals helped me appreciate how useful signal processing can be beyond engineering: in neuroscience, medicine, cognitive research, and more. Even a basic filter or transform can uncover structure in what looks like noise.

This wasn’t just about finishing an assignment—it was about connecting theory to something alive, literally. Seeing how an FIR filter reveals an Alpha wave or how convolution alters a brain signal gave me a new appreciation for the tools we’re learning.

---

## What I Learned

This project started as a homework assignment, but honestly, I really enjoyed working on it. Even though I already knew some MATLAB, this project challenged me to learn a lot more—especially when dealing with EEG data and Phase-Amplitude Coupling concepts. It pushed me to dig deeper into signal processing and explore new techniques I hadn’t used before.

I also got more comfortable with LaTeX while putting together the report, which was a nice bonus. All in all, it was a great chance to improve both my coding and documentation skills.

Looking back, I’m glad I stuck with it. It showed me that even if something seems tough at first, with patience and practice, you can learn a lot—and maybe even enjoy it along the way!


 --- 

 
## Data Structure

For each phase of the project, I organized everything into three main files:

- **Phase1_Report.pdf** — This is the full report for Phase 1, where I explain the goals, methods, results, and conclusions.
- **Phase1_Code.zip** — All the code and scripts used for Phase 1 are inside this archive. The folders are structured to make it easy to follow.
- **Phase1_Results.zip** — Here you'll find the results, including output data, charts, and any figures generated from running the code.

The same format is used for Phase 2:

- **Phase2_Report.pdf**
- **Phase2_Code.zip**
- **Phase2_Results.zip**

This way, everything related to each phase is grouped together, making it straightforward to access the reports, code, and results without confusion.


## Course Context

**Course:** Signals and Systems  
**Instructor:** Professor Hamid Karbalaei Aghajan  
**University:** Sharif University of Technology  
**Department:** Electrical Engineering 1  
**Semester:** Spring 2025

