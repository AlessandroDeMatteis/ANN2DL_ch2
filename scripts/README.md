Hi, it’s arialeto here!

This folder contains some of the scripts developed during this challenge, together with the related report.
Each script is named after the corresponding architecture and techniques used, and implements both transfer learning and fine‑tuning.
All scripts are runnable: simply provide a dataset folder named clean_patches, open the notebook, and execute the cells.

In addition, we include a script called "Patches_extractor", used to create the patches employed during training.

Finally, there is a PDF file called "Extra", where we describe an attempt to implement a dual‑network setup: one model trained on patches and another on full‑resolution images using a lazy‑dataset architecture. Unfortunately, this approach did not yield significant improvements in our experiments.
