# Enterprise-ML-Recommender-Analytics-Suite
A multi-threaded data science workbench built in pure Python (Tkinter) that bridges theoretical algorithm complexity with real-world machine learning. This suite ingests sparse datasets (e.g., MovieLens), trains recommendation models, and utilizes the resulting matrices to conduct dynamic multithreading CPU stress tests.

🚀 Features
• Interactive Data Insights: Automated parsing of CSV datasets with visual analytics for rating distributions and matrix sparsity.

• Machine Learning Pipeline:

  • Latent Factor Models utilizing parallelized Stochastic Gradient Descent (SGD).

  • Cosine-based Collaborative Filtering (User-User and Item-Item similarity).

• Real-time Model Evaluation: Visualizes gradient descent optimization through live loss curves and evaluates test-set accuracy via Error Distribution charts and RMSE.

• Performance Benchmarking: Evaluates computational overhead by executing $O(N^3)$ matrix workloads across different threading strategies:

  • Single-threaded (Sequential)

  • Coarse-grained parallelism (Thread-per-Row)

  • Managed Thread Pool Execution (Hardware-tuned)

🛠️ Installation & Setup
1. Clone the repository:

```

git clone https://github.com/[your-username]/Enterprise-ML-Recommender.git

cd Enterprise-ML-Recommender

```

2. Run the application (no external dependencies required):

```

python recommender_dashboard_v4.py

```

3. Download a dataset (e.g., MovieLens ml-latest-small) and load the `ratings.csv` file within the application's Data Insights tab.(You can use any dataset as long as they have a rating.csv with the format mentioned in the upload section of the code.)

🧠 Core Engineering Concepts Demonstrated
• Algorithm Optimization: Implementing Machine Learning algorithms (SGD) from scratch to understand matrix decomposition.

• Concurrency Analysis: Benchmarking the effects of the Global Interpreter Lock (GIL) and measuring OS context-switching overhead during heavy mathematical workloads.

• GUI Thread Safety: Utilizing asynchronous background workers to ensure UI responsiveness during prolonged CPU calculations.

📷 Application Previews

• `[Screenshot of Tab 1: Data Insights]`
(Add screenshots of your application here)<img width="1920" height="1080" alt="Screenshot (80)" src="https://github.com/user-attachments/assets/33d6c16e-e5d3-4896-93d1-1b058a71a2a1" />


• `[Screenshot of Tab 2: Live ML Training]`
<img width="1920" height="1080" alt="Screenshot (81)" src="https://github.com/user-attachments/assets/41e8c225-c74e-4e2f-90e9-b6d19f345cd3" />


• `[Screenshot of Tab 3: Engine Benchmark]`
<img width="1920" height="1080" alt="Screenshot (82)" src="https://github.com/user-attachments/assets/fc8fa989-6889-451f-8347-9dc256f0d04d" />

The Entirety of Code was handwritten over the course of a week as a part of mini-project for DAA subject. No AI was used for code writing except Code beautification and quality of life additions in the code.

👨‍💻 Author
Shashank Sanjay Dattu 
