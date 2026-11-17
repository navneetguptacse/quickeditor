# QuickEditor — Official Product Landing Page

[![ourcrepe](https://img.shields.io/badge/ecosystem-ourcrepe-3178c6?style=flat)](https://ourcrepe.live)
[![QuickEditor](https://img.shields.io/badge/QuickEditor-Coming%20Soon-d97706?style=flat&logo=visualstudiocode&logoColor=white)](https://quickeditor.ourcrepe.live)
[![QuickRunner](https://img.shields.io/badge/QuickRunner-Live-059669?style=flat)](https://quickrunner.ourcrepe.live/)
[![License: MIT](https://img.shields.io/badge/license-MIT-0f2744?style=flat)](https://opensource.org/licenses/MIT)
[![Supported Platforms](https://img.shields.io/badge/platforms-Codeforces%20%7C%20LeetCode%20%7C%20AtCoder-4a90e2?style=flat)](https://quickeditor.ourcrepe.live)

High-performance, minimalist product landing page and interactive sandbox for **QuickEditor**, the AI-augmented contest code editor in the **ourcrepe** developer tooling ecosystem.

Styled with the exact clean aesthetic, typography, and theme system of [ourcrepe.live](https://ourcrepe.live) and [quickrunner.ourcrepe.live](https://quickrunner.ourcrepe.live/).

---

## What is QuickEditor?

**QuickEditor** is an AI-powered code editor engineered specifically for competitive coders and algorithm builders (Codeforces, LeetCode, AtCoder, CSES, USACO, ICPC):

- **Automated Dual Stress-Testing**: Automatically fuzzed against naive brute-force solutions on randomized inputs to isolate minimal failing counterexamples.
- **AI Edge-Case Hunter**: Pre-scans problem constraints and logic for off-by-one errors, 32-bit integer overflow, disconnected graphs, precision traps, and empty inputs.
- **Big-O Constraint & TLE Guard**: Real-time evaluation of time/space complexity against problem time limits (e.g. verifying `O(N log N)` within 1.0s limit for `N ≤ 2 × 10⁵`).
- **Contest Platform Parsing**: One-click URL import for Codeforces, LeetCode, and AtCoder problems and test case suites.
- **Progressive Algorithmic Hints**: Multi-tier hinting (Observation &rarr; Data Structure &rarr; Pseudo-code) that guides without spoiling.
- **100% Offline & Private**: Zero code telemetry. Solutions and contest strategies run locally on your machine with sub-millisecond latency.

---

## Products & Ecosystem

| Product | Status | Primary URL | Description |
| :--- | :--- | :--- | :--- |
| **ourcrepe** | Live Hub | [ourcrepe.live](https://ourcrepe.live) | Parent developer tooling ecosystem for minimalist, high-speed utilities. |
| **QuickRunner** | Live | [quickrunner.ourcrepe.live](https://quickrunner.ourcrepe.live/) | All-in-one code runner for VS Code & terminal across 60+ languages with zero setup. |
| **QuickEditor** | Coming Soon (Active Dev) | [quickeditor.ourcrepe.live](https://quickeditor.ourcrepe.live) | AI-powered code editor engineered for competitive coders featuring automated stress-testing and edge-case generation. |

---

## Theme & Design Details

- **Typography**: 
  - **Inter**: Modern UI sans-serif for body, headers, and navigation.
  - **JetBrains Mono**: Terminal code blocks, tabs, testcases, shortcuts, and badges.
  - **Pinyon Script**: Signature cursive accents (`"Simple, fast, contest-first"`).
- **Brand Assets**:
  - `images/logo.png`: High-resolution **ourcrepe** / **QuickEditor** emblem with blue gradient drop shadow.
  - `favicon.ico` & `images/logo.ico`: Multi-resolution icon resource (16x16, 32x32, 48x48, 64x64) for browser tabs and bookmarks.
- **Vector Icons (Font Awesome 6)**:
  - Vector icons used exclusively throughout the UI (theme toggles, external link indicators, feature grid, and card badges). Zero raw emojis.
- **Light & Dark Mode**:
  - Automatically respects system appearance (`prefers-color-scheme`).
  - Interactive theme toggle button in the navigation header with local storage persistence (`quickeditor_theme` and fallback `ourcrepe_theme`).
- **Interactive Sandbox & Playground**:
  - Multi-tab code editor (`Solution.cpp`, `BruteForce.cpp`, `Generator.py`).
  - Problem presets (Maximum Subarray XOR, Two Pointers & Slimes, Shortest Path with Tolls).
  - Simulated test execution, live 100-run dual stress-testing bar, progressive hint revealer, and edge-case injector.
- **Zero Dependencies**: Pure HTML, CSS, and vanilla JS — zero build steps or heavy node frameworks.
---

## Local Development & Preview

You can preview the site directly in any browser:

### Option 1: Local HTTP Server (Recommended)
Using Python (pre-installed on macOS/Linux):
```bash
python3 -m http.server 3000
```
Then open [http://localhost:3000](http://localhost:3000) in your browser.

Using Node / npx:
```bash
npx serve .
```

### Option 2: Direct File
Double-click `index.html` to open it directly in Chrome, Safari, or your preferred browser.

---

## Deployment

Since this is a lightweight static site with a `CNAME` file, you can deploy it in seconds:

- **GitHub Pages**:
  1. Push this repository to GitHub (`navneetguptacse/quickeditor`).
  2. Go to **Settings > Pages**.
  3. Set Source to `Deploy from a branch` and select `main` / `/ (root)`.
  4. Ensure Custom Domain points to `quickeditor.ourcrepe.live`.
- **Cloudflare Pages / Vercel / Netlify**:
  - Connect your Git repository with build command left empty and publish directory set to `/`.
