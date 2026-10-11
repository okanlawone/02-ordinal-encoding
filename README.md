# Project 2: Make and defend an encoding choice

Compare one-hot encoding for unordered departments with ordinal codes for condition labels, then explain why the category order must come from meaning rather than alphabetical order.

**Repository:** [okanlawone/02-ordinal-encoding](https://github.com/okanlawone/02-ordinal-encoding)  
**Course index:** [ai-engineering-journey](https://github.com/okanlawone/ai-engineering-journey)

## What you will learn

- Distinguish nominal categories from categories that have a meaningful order.
- Compare an explicit dictionary mapping with scikit-learn’s `OrdinalEncoder`.
- Show that the supplied category list determines the integer codes.

## Project format

This is an open-ended, multi-session project. The starter program demonstrates the core idea; your work is to inspect it, extend it, and explain the choices. There is no one-day deadline. Pick up at the next unchecked item in [`progress.md`](progress.md). The detailed background and project brief are in [`lesson.md`](lesson.md).

## Checkpoints

- [ ] **Sort categories by meaning:** For each categorical column, explain whether its labels have an inherent order.
- [ ] **Inspect both representations:** Run the baseline and locate the department indicator table, the manual condition mapping, and the ordinal-encoder output.
- [ ] **Check the order explicitly:** Verify that the intended condition progression is `Poor < Fair < Good < Excellent`, with codes increasing in that order.
- [ ] **Run a counterexample:** Change the explicit category order in a temporary experiment and explain why the codes change even though the observations do not.
- [ ] **Write an encoding decision:** For each column, state the chosen encoding and the meaning—or lack of meaning—of the resulting numbers.

## Run the starter project

Clone this project repository, then run these commands from its root:

```bash
git clone https://github.com/okanlawone/02-ordinal-encoding.git
cd 02-ordinal-encoding
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python main.py
```

The code reads its CSV from the project folder, so it does not depend on your terminal’s current directory. The small CSV is invented practice data; it is not real customer data. See [`lesson.md`](lesson.md) for the data and training-data distinction.

## What counts as complete

Use the checklists in `lesson.md` and `progress.md`. A project is ready to close when the required behavior works, you can explain why the choices make sense, and the data limitations are documented. Optional extensions can wait for a later version.

**Optional extension:** Look up how an encoder can handle a category it did not see while fitting. Explain why that question matters when a model later receives new records; do not silently assign a new label an arbitrary rank.
