# 🖨️ CoachPrint Suite

CoachPrint Suite is a high-performance, 100% browser-based PDF utility designed specifically for students, educators, and professionals who want to optimize, prune, and prepare lecture notes and coaching slides for physical printing. 

It solves a major pain point in digital learning: **saving printer toner** when printing dark-themed presentation slides, while giving you complete control over document structure and multi-file merging.

---

## ✨ Key Features

* **🎨 Smart Structural Recognition:** Automatically parses uploaded PDF coaching decks to identify **Cover pages** (Page 1), **Summary slides**, and **Closing/Thank-You cards** on initial load.
* **💡 Toner Inversion Optimization:** Instantly inverts dark slide backgrounds to clear white, drastically reducing black toner consumption for printing.
* **✂️ Page Pruning & Reordering:** Easily remove unwanted blank or redundant slides with a single click. Every card displays both its current sequence position and original source page number.
* **🏷️ Manual Role Overrides:** Change page roles (Cover, Body, Summary, Closing) with automatic fallback inversion toggles.
* **🔗 Multi-PDF Merger:** Combine multiple lecture modules, notes, or assignment PDFs into a single sequential document with zero server upload.
* **🖥️ Display Scale Auto-Adjustment:** Automatically detects high-density or scaled OS display settings (e.g., Windows 125% or 150%) and counters zoom to fit your monitor screen perfectly.
* **🌙 Comfortable Theme Engine:** Features an eye-friendly **Catppuccin** palette with a seamless Light/Dark mode switcher.
* **🔒 100% Private & Local:** Runs entirely client-side inside your browser via WebAssembly and JavaScript engines. Your files never leave your machine.

---

## 🚀 Quick Start / Usage

Because CoachPrint Suite is bundled into a single standalone architecture, running it requires no complex backend servers, installations, or build pipelines.

1. Download or save the application code as **`index.html`**.
2. Double-click the file to open it in any modern browser (**Chrome, Edge, Safari, or Firefox**).
3. Choose your workflow:
   * **Print Optimizer Mode:** Drag and drop your coaching PDF to inspect, prune, invert tones, and download a print-ready version.
   * **Merge PDFs Mode:** Select multiple PDF files to combine them into an ordered single document.

---

## 🛠️ Technology Stack

* **[Vue.js 3 (CDN)](https://vuejs.org/):** Reactive single-page application framework for instant UI updates and state management.
* **[Tailwind CSS (CDN)](https://tailwindcss.com/):** Modern utility-first styling with custom theme definitions.
* **[PDF.js](https://mozilla.github.io/pdf.js/):** Mozilla's robust client-side rendering engine used for layout parsing and high-res canvas thumbnail generation.
* **[pdf-lib](https://pdf-lib.js.org/):** Pure JavaScript library used for assembling, copying, compressing, and merging raw PDF streams.

---

## ⚙️ Export Quality Presets

When downloading your optimized PDF, you can choose between two rendering configurations:
* **Standard Quality:** Uses 1.5x scaling with optimized JPEG compression (~80% quality) to ensure a lean, printer-friendly file size.
* **High Quality:** Uses 2.2x high-DPI scaling (~92% quality) for maximum vector/image sharpness.

*Note on Inversion:* Inverted pages are converted to high-resolution JPEG streams to invert their color pixels, while untouched body pages remain native vectors.

---

## 📄 License

This project is open-source and available for personal, educational, and commercial productivity use. Feel free to modify and adapt it to your workflow!
