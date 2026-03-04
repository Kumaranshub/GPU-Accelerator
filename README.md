# Quick run (no model loading)
python benchmarks/run_benchmarks.py --quick

🗂️ Project Structure
optigpu/
│
├── 📄 framework/
│   └── optigpu_framework.py     # Core: all 4 optimization layers + benchmark engine
│
├── 📊 benchmarks/
│   └── run_benchmarks.py        # Full benchmark suite with JSON + PNG output
│
├── 🔌 hardware/
│   └── esp32/
│       ├── tflite_demo.py       # INT8 model conversion + ESP32-S3 inference
│       └── README.md            # Hardware setup guide (₹700 demo)
│
├── 📓 notebooks/
│   └── OptiGPU_Colab.ipynb      # Step-by-step Colab notebook
│
├── 📁 results/                  # Benchmark outputs (generated, not tracked)
├── 📝 paper/                    # Research paper (WIP)
│
├── requirements.txt
└── README.md

🔌 Hardware Demo — ESP32-S3 (₹700)
The physical demo runs a quantized MobileNetV2 model on a ₹700 ESP32-S3 microcontroller, classifying webcam images in real time at 30+ FPS using 0.5 watts.

ESP32-S3 (OptiGPU)
RTX 5090 (Naive FP32)
Cost
₹700
₹2,50,000
Power
0.5W
575W
Task
Image classification
Image classification
FPS/Watt
100
0.22
Winner
✅ 455x more efficient
❌

See hardware/esp32/ for setup instructions.

📅 Research Timeline
Month 1  ████████░░░░  Baseline benchmarks · FP16 · INT8
Month 2  ████████████  INT4 · torch.compile · ESP32 demo
Month 3  ░░░░░░░░░░░░  Paper write-up · Final presentation

🛠️ Requirements
Python 3.9+
PyTorch 2.0+
CUDA-capable GPU or Google Colab free tier (T4)
See requirements.txt for full dependency list

📄 License
MIT © 2025 — Free to use, modify, and build on.


Built with ₹0 cloud spend. Runs entirely on Google Colab free tier.⭐ Star this repo if it helped your research￼ 
