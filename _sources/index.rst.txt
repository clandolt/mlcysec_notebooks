.. CISPA Machine Learning in Cybersecurity documentation master file, created by
   sphinx-quickstart on Wed Oct  8 17:26:56 2025.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

CISPA Machine Learning in Cybersecurity tutorials
=================================================



📘 Course Information
=====================

| **Course website:** `Course website <https://cms.cispa.saarland/mlcysec_ws25/>`_
| **Course edition:** Winter term 2025/2026 (Oct 13 – Feb 06)
| **Recordings:** Will follow
| **Instructor:** Christoph R. Landolt

---

⚙️ How to Run the Notebooks
===========================

The website hosts HTML-exported versions of the notebooks for convenient reading on any device.  
However, we encourage you to run them yourself to gain hands-on experience.  
You can do this in three main ways:

🖥️ Run Locally (CPU)
--------------------
All notebooks are available in this GitHub repository.  
You can also find them here:  
👉 `GitHub repository <https://github.com/clandolt/mlcysec_notebooks>`_

- Designed to run on standard laptops (no GPU required).

☁️ Google Colab
---------------
Prefer to use a hosted environment or want GPU support? Use [Google Colab](https://colab.research.google.com/notebooks/intro.ipynb#recent=true).

- Each notebook includes a “Run in Colab” badge on the documentation website.
- Enable GPU support via: `Runtime → Change runtime type → GPU`.

---

🧭 Tutorial Lessons
===================

The **Exercise Schedule** (below) lists the practical/tutorial sessions associated with the course tutorials.
The sessions will take place in **CISPA Lecture Hall, Stuhlsatzenhaus 5**.

+------------+------------+------------------------------------------------+
| **Date**   | **Time**   | **Topic**                                      |
+============+============+================================================+
| 29.10.2025 | 16:15-17:45| Tutorial: ML Basics / Setup                    |
+------------+------------+------------------------------------------------+
| 05.11.2025 | 16:15-17:45| Q&A: ML Basics                                 |
+------------+------------+------------------------------------------------+
| 12.11.2025 | 16:15-17:45| Introduction Ex1: Train ML IDS                 |
+------------+------------+------------------------------------------------+
| 03.12.2025 | 16:15-17:45| Ex1 Review: Train ML IDS                       |
+------------+------------+------------------------------------------------+
| 10.12.2025 | 16:15-17:45| Introduction Ex2: Evade ML IDS                 |
+------------+------------+------------------------------------------------+
| 07.01.2026 | 16:15-17:45| Ex2 Review: Evade ML IDS                       |
+------------+------------+------------------------------------------------+
| 14.01.2026 | 16:15-17:45| Introduction Ex3: AI for CTF                   |
+------------+------------+------------------------------------------------+
| 04.02.2026 | 16:15-17:45| Ex3 Review: AI for CTF                         |
+------------+------------+------------------------------------------------+




---

💬 Feedback, Questions, or Contributions
========================================

This is the first edition of the **Machine Learning in Cybersecurity** tutorials.  
We appreciate all feedback — whether it’s a typo, a bug, or a suggestion for improvement.

If you discover a **mistake or issue in a notebook**, please [open a GitHub issue](../../issues) so we can track and resolve it publicly.

You can also reach out directly via email (`christoph dot landolt at cispa dot de`), or speak to us during a exercise session.

If you find the tutorials helpful, please cite this course as:

.. code-block:: bibtex

  @misc{landolt2025_mlcysec,
    title        = {CISPA Machine Learning in Cybersecurity},
    author       = {Christoph R. Landolt and Mario Fritz},
    year         = {2025},
    howpublished = {\url{https://christophlandolt.com/mlcysec_notebooks/}},
  }


.. toctree::
   :maxdepth: 2
   :caption: Tutorial 1: Getting started:

   tutorial_notebooks/getting_started_with_jupyter_and_python/getting_started_with_jupyter_and_python
   tutorial_notebooks/discover_visualize_gain_insights/discover_visualize_gain_insights
   tutorial_notebooks/getting_started_with_ml/getting_started_with_ml
   tutorial_notebooks/getting_started_with_deep_learning/getting_started_with_deep_learning

.. toctree::
   :maxdepth: 2
   :caption: Tutorial 2: Intrusion Detection and Response Systems:


   .. toctree::
   :maxdepth: 2
   :caption: Tutorial 2: Evading Machine Learning-based IDS:


   .. toctree::
   :maxdepth: 2
   :caption: Tutorial 4: ML in the hands of Attackers (CTF):