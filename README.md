# Minor-project-1
# GroupDNA: WhatsApp Group Chat Analyzer

A pure Python and NumPy-based analytics tool designed to clean, parse, and analyze unstructured raw WhatsApp chat export logs.

This project was built entirely from scratch under strict structural constraints, avoiding common data libraries to showcase algorithmic fundamentals, data engineering, and matrix operations.

## 📌 Project Architecture & Constraints

To demonstrate strong foundational programming skills, this project strictly avoids high-level data frameworks. The analytical pipeline adheres to the following environment rules:
* **No Pandas:** Built entirely with core Python loops, data types (lists, dicts, sets), and native file handling.
* **No Regular Expressions (re):** All log text slicing and message cleaning are done using native string manipulation methods.
* **No Collections Module:** Item frequency sorting is computed using custom sorting loops rather than `collections.Counter`.
* **No Plotting Libraries:** Skips graphical toolkits like `matplotlib` or `seaborn`, creating a rich visual dashboard right inside the terminal text grid.
* **Mathematical Core:** Utilizes standard **NumPy matrices and arrays** to map multidimensional group behavior.

## 📊 8 Core Features Implemented

The notebook runs an automation pipeline that successfully computes all eight mandatory metrics requested in the project brief:

1. **Feature 1: The Chat Parser** – Automatically extracts dates, times, sender profiles, and message contents while filtering structural anomalies like media stubs, deleted flags, and multi-line conversation blocks.
2. **Feature 2: Group Overview** – Computes the group lifetime timeline, total message volumes, unique participant counts, and relative communication volumes per member.
3. **Feature 3: Busiest Timings** – Tracks timestamp indices to pinpoint the single absolute peak date and most active hour of the day for the group.
4. **Feature 4: Activity Heatmap Matrix** – Constructs a **6x24 NumPy matrix** (6 participants by 24 hourly buckets). It renders a dense text chart directly in the console using block shading symbols (`.`, `,`, `░`, `█`) based on messaging densities.
5. **Feature 5: Word Cloud Text Analysis** – Normalizes string logs into clean tokens by lowercasing text, dropping standard punctuation characters, filtering out common stop words, and generating a text-bar chart of the top 10 most used words.
6. **Feature 6: Response Speeds & Silent Streaks** – Uses temporal differences to compute individual average response times between chat entries and tracks the longest inactive periods per user.
7. **Feature 7: Personality Archetype Engine** – Implements a heuristic scoring system to assign group personalities (e.g., *THE SPAMMER, THE NIGHT OWL, THE STORYTELLER, THE DRAMA QUEEN*) based on unique behavioral metrics.
8. **Feature 8: Final Formatted Report** – Formats the final output dashboard using clean decorative borders (`=`, `-`) and padding rules (`f'{name:<10}'`) for a pristine layout.

## 📂 Repository Layout

* `GroupDNA_POOJA S_4SM22EC065.ipynb` — The primary Jupyter Notebook containing the clean source code pipeline and executed console dashboard.
* `hostel_bois.txt` — The raw, exported WhatsApp chat text history file used as the data source.

---
*Developed as part of academic minor project requirements by Pooja S (Roll Number: 4SM22EC065).*
