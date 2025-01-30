# Manim LLM Pipeline with Program-aided Language (PaL)

## 🚀 Project Overview

This project aims to generate **Manim animations** that visually explain **basic algebra problems and their solutions**, leveraging **SymPy as a symbolic solver** and **LLM-based prompt engineering using the PaL (Program-aided Language) technique**.

The pipeline follows these steps:

1. **User Input**: An algebra problem (e.g., `x^2 - 4 = 0`).
2. **SymPy Processing**: Solves the equation and structures step-by-step output.
3. **PaL Prompting**: Converts structured steps into a precise prompt for an LLM.
4. **Manim Code Generation**: The LLM produces a Manim script.
5. **Animation Rendering**: Runs the Manim script to generate an educational video.

## 🛠️ Tech Stack

- **Manim** – For mathematical animations.
- **SymPy** – For symbolic algebra processing.
- **LLM (GPT-4 Turbo, etc.)** – For structured prompt-based code generation.
- **Python** – Core programming language.

## 📂 Project Structure

```
📁 manim_pal_pipeline
│── 📁 src
│   │── sympy_solver.py         # Algebra solver using SymPy
│   │── pal_prompt.txt          # Prompt template for LLM
│   │── generated_manim.py      # LLM-generated Manim script
│   │── final_manim.py          # Final optimized Manim animation
│── README.md                   # Project documentation
```

## ⚡ Getting Started

### **1. Clone the Repository**

```bash
git clone https://github.com/yourusername/manim_pal_pipeline.git
cd manim_pal_pipeline
```

### **2. Install Dependencies**

```bash
pip install sympy manim openai
```

### **3. Solve an Algebra Problem Using SymPy**

```bash
python src/sympy_solver.py
```

### **4. Generate a Manim Script Using PaL**

- Manually test `src/pal_prompt.txt` with an LLM.
- Paste the output into `src/generated_manim.py`.

### **5. Render the Manim Animation**

```bash
manim src/generated_manim.py SolveEquation -pql
```

## 🛠️ Future Improvements

- Automate the **LLM API call → Manim script generation → Video rendering**.
- Expand to **calculus, geometry, and physics problems**.
- Improve prompt engineering to **enhance code clarity**.

## 🤝 Contributing

1. **Fork the repo** and create a new branch.
2. Submit a **pull request** with clear descriptions.
3. **Join discussions** in Issues/PRs for improvements.

## 📜 License

MIT License – Free to use and modify.

---

### 🎯 The goal: **Make math visually intuitive through AI-powered animations!** 🚀

