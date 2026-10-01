# Hi, I'm Soroush Zandi Esfahani

**Robotics & ML engineer · MASc candidate in Engineering Science at Simon Fraser University (graduating Dec 2026)**

I build robot manipulation systems that combine learned policies with force control. My background is in electrical engineering (BASc, electronics), and my current work sits between robotics, machine learning, and software. I'm looking for roles in **robotics, machine learning, electrical engineering, and software engineering**.

[![Email](https://img.shields.io/badge/Email-soroushznd78%40gmail.com-D14836?logo=gmail&logoColor=white)](mailto:soroushznd78@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-soroush--zandi-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/soroush-zandi/)
![Location](https://img.shields.io/badge/Location-BC%2C%20Canada-555)

---

## 🔪 Current research: BLADE (MASc thesis)

**Robotic fruit cutting with a Kinova Gen3 7-DOF arm**, combining a diffusion model, a library of motion primitives, and force control.

**Robotics & control**
- Built a **ROS 2 Humble** control stack for the Kinova Gen3 (Kortex, `ros2_control`, MoveIt 2) with a **Robotiq gripper** and **force/torque sensing** (`force_torque_sensor_broadcaster`).
- Built a **primitive library** of force-controlled cutting motions.
- Implemented a **500 Hz admittance controller**, based on published research, with a contact model for fruit and cutting board.
- Designed a **dual-rate control loop**: 500 Hz force control, 30 Hz inverse kinematics, and a 12 Hz state machine.
- Wrote a **custom deterministic IK solver with PyKDL** to replace MoveIt's default plugin, and built a custom MoveIt configuration for the arm.
- Debugged simulation bring-up (URDF/xacro, controller YAML, launch files). For example, I traced a Robotiq xacro failure (`isaac_joint_commands`) to the gripper configuration after confirming the arm-only setup worked.

**AI & perception**
- Built a **two-tier vision pipeline**: a vision-language model plans each cut, and a lightweight OpenCV monitor watches for problems during motion, calling the full model only when needed.
- Wrote a cut-plan parser that works with both the **Claude and OpenAI APIs** and returns **structured output**.
- Wrote a data logger that records every cut as training data for a **diffusion policy**. Fine-tuning **RDT-1B**, a robotics diffusion foundation model, is *in progress*.

**Simulation & tooling**
- Adapted a published research codebase into a knife-cutting simulation in **ManiSkill / SAPIEN** with soft-body physics (**MPM**).
- Built a live telemetry dashboard with **Flask, Server-Sent Events, and Chart.js**.
- Set up GPU-accelerated simulation on Linux, including NVIDIA drivers under Secure Boot.

**Research**
- Compared 19 robotics papers, checking each claim against its source, and found errors in published claims.
- Wrote the thesis proposal and presented research papers to my supervisor.

---

## 🧠 Selected projects

| Project | What I did | Stack |
|---|---|---|
| **Aerial image segmentation (iSAID)** | Trained and debugged a semantic segmentation model on the iSAID dataset; **mean IoU 0.7629** | PyTorch, Detectron2, CUDA, T4/A100 GPUs |
| **Brain tumor MRI classification** | Compared CNN classifiers on a Kaggle MRI dataset: **VGG16 98.43%**, **EfficientNetV2 98.78%** accuracy | PyTorch / deep learning |
| **Reinforcement & imitation learning** (CMPT 729) | Implemented Behavioral Cloning, DAgger, Cross-Entropy Method, DQN, and Policy Gradient | Python, PyTorch |
| **AI document automation** (IMM Recruitment) | Computer-vision pipeline to digitize documents and extract and validate structured data | OpenCV, YOLO, TensorFlow (CNNs, ViT), CUDA |

---

## 💼 Experience

**Exam Invigilator**, Centre for Accessible Learning (CAL), Simon Fraser University · *Summer 2025 – present*
- Supervise exams for students with academic accommodations.

**Data Entry Specialist (AI Integration)**, IMM Recruitment · *Mar 2024 – present*
- Built OpenCV and YOLO pipelines to automate document digitization.
- Trained TensorFlow vision models (CNNs, Vision Transformers) to extract and validate structured data from unstructured documents.
- Added CUDA-accelerated inference for faster processing of scanned documents.

**Research Assistant**, Sepahan Road Construction Company · *Apr – Dec 2023*
- Designed PCB layouts (Altium Designer) and ran power-electronics simulations (LTspice) for asphalt-plant automation.
- Developed ARM Cortex-M prototypes for electronic devices.

**Intern**, Technical and Vocational Training Organization · *Feb – Apr 2021*
- Programmed PLC-based elevator controllers using C/C++ and Assembly.

---

## 🎓 Teaching

**Simon Fraser University, Teaching Assistant**
- **ENSC 151: Intro to Software Development** *(Fall 2026, Fall 2024)*. C++, OOP, data structures, Linux, Git.
- **ENSC 252: Digital Logic & Design** *(Fall 2026, Fall 2024)*. VHDL, FPGA prototyping, Quartus Prime, ModelSim.
- **ENSC 406: Engineering Ethics.** Designed 50-minute discussion tutorials on ethical frameworks and case studies (Therac-25, Ford Pinto).
- **ENSC 351.**
- **ENSC 280: Engineering Measurement & Data Analysis** *(Summer 2025)*. Data analysis, error measurement, and MATLAB labs with sensors and circuits.
- **ENSC 325: Microelectronics II, Head TA** *(Spring 2025)*. MOSFET/CMOS/BJT amplifier labs and SPICE simulation.
- Graded 75 student design submissions against a sustainability rubric.

**University of Isfahan, TA for Physics & Mathematics** *(2021–2022)*

---

## 🛠️ Skills

- **Robotics:** ROS 2 Humble, MoveIt 2, ros2_control, Kinova Kortex, PyKDL, URDF/xacro/SRDF, Gazebo, RViz, admittance/force control, PID, MPC
- **Machine learning:** PyTorch, TensorFlow, Detectron2, CUDA, diffusion policies (RDT-1B), reinforcement & imitation learning, LLM APIs (Claude, OpenAI) with structured output
- **Computer vision:** OpenCV, YOLO, Vision Transformers, semantic segmentation
- **Simulation:** ManiSkill / SAPIEN (MPM), Gazebo, NVIDIA Omniverse, Unity, Unreal Engine
- **Languages:** Python, C++, C, MATLAB, R, Assembly, VHDL, SystemVerilog, Java (basic)
- **Hardware & EE:** ARM Cortex-M, FPGA, PLC, Altium Designer, OrCAD, LTspice, PCB layout
- **Software & tools:** Linux, Git, Flask, Server-Sent Events, Chart.js, LaTeX

---

## 🎓 Education

- **MASc, Engineering Science**, Simon Fraser University · *Jan 2024 – Dec 2026*
- **BASc, Electrical Engineering (Electronics)**, University of Isfahan · *Sep 2018 – Jan 2023* · GPA 3.54
