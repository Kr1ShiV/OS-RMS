# OS-RMS: Interactive OS Resource Management System

> A complete, production-ready, single-file interactive web simulator for core Operating System algorithms — built for 3rd-year CS students and academic evaluators.

**🔗 Live Demo:** Open `index.html` directly in any browser — no server, no install, no build step needed.

---

## 🚀 Features

### 🖥️ Module 1 — CPU Scheduling
Simulate and benchmark four classic CPU scheduling algorithms:

| Algorithm | Type |
|-----------|------|
| **FCFS** (First-Come, First-Served) | Non-preemptive |
| **SJF** (Shortest Job First) | Non-preemptive |
| **SRTF** (Shortest Remaining Time First) | Preemptive |
| **Round Robin** | Preemptive, configurable time quantum (1–10) |

**Outputs:**
- 🎨 Color-coded interactive **Gantt Chart** with hover tooltips
- 📊 Performance table: CT, TAT, WT per process
- 📈 Metrics: Avg Waiting Time, Avg Turnaround Time, CPU Utilization %, Throughput

---

### 🧠 Module 2 — Contiguous Memory Allocation
Simulate three primary memory partitioning strategies:

| Strategy | Description |
|----------|-------------|
| **First Fit** | Allocates the first block large enough |
| **Best Fit** | Allocates the smallest sufficient block |
| **Worst Fit** | Allocates the largest available block |

**Outputs:**
- 🗺️ Visual **RAM partition map** (allocated, internal fragmentation, free)
- 📋 Allocation ledger with per-process block assignment
- 📊 Summary: Total RAM, Allocated, Free Space, Internal Fragmentation

---

### 📄 Module 3 — Virtual Memory Page Replacement
Simulate three page replacement algorithms:

| Algorithm | Description |
|-----------|-------------|
| **FIFO** | Evicts the oldest loaded page |
| **LRU** | Evicts the least recently used page |
| **NRU / Clock** | Uses R (Referenced) and M (Modified) bits; evicts lowest-class page |

**Outputs:**
- 🗃️ Step-by-step **Frame Matrix table** — every memory access visualized
- 🟢 HIT / 🔴 FAULT badges per step
- Eviction reason per fault (e.g., LRU timestamp, NRU class R/M bits)
- 📊 Metrics: Total Requests, Page Faults, Page Hits, Hit Ratio %, Miss Ratio %

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Markup | HTML5 |
| Styling | Tailwind CSS (CDN) |
| Logic | Vanilla ES6+ JavaScript |
| Icons | Lucide Icons (CDN) |
| Backend | None — 100% client-side |

---

## 📂 Project Structure

```
OS-RMS/
└── index.html   ← entire application (HTML + CSS + JS, ~52 KB)
```

---

## ▶️ How to Run

### Option 1 — Direct Open (Recommended)
Double-click `index.html` → opens in your default browser. Done.

### Option 2 — GitHub Pages
1. Fork this repository
2. Go to **Settings → Pages**
3. Set source to `main` branch, root `/`
4. Your app will be live at `https://<your-username>.github.io/<repo-name>/`

### Option 3 — Any Local Server
```bash
# Python
python -m http.server 8080

# Node.js (npx)
npx serve .
```

---

## 🎓 Academic Use

This simulator is designed for:
- **CS Lab Assignments** — compare algorithm performance on custom inputs
- **Exam Preparation** — visualize algorithm execution step by step
- **Project Demos** — load preset data and present with one click
- **Teaching Aid** — project on screen and walk through each step

---

## 🤝 Contributing

Pull requests are welcome! To contribute:

1. **Fork** the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add: your feature description"`
4. Push to your branch: `git push origin feature/your-feature`
5. Open a **Pull Request**

### Ideas for Contribution
- [ ] Add **Priority Scheduling** algorithm to CPU module
- [ ] Add **Optimal (OPT)** page replacement algorithm
- [ ] Add **Worst Fit Decreasing** strategy to memory module
- [ ] Export results as CSV or PDF
- [ ] Add animation/step-through mode for Gantt chart
- [ ] Add dark/light theme toggle

---

## 📄 License

MIT License — free to use, modify, and distribute for academic and personal projects.

---

## 👨‍💻 Authors

Built with ❤️ for Operating Systems coursework.
