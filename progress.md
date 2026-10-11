# Project 2: Make and defend an encoding choice — progress

**Guide status:** The starter files and project brief are published. Learner work on the open-ended checkpoints has not been verified, so the learning checklist starts unchecked.

Use this page across sessions. Check an item only after you have done it and can explain what you learned. If a step takes more than one sitting, leave it unchecked and write your next small move in the session log.

## Checkpoints

- [ ] **Sort categories by meaning:** For each categorical column, explain whether its labels have an inherent order.
- [ ] **Inspect both representations:** Run the baseline and locate the department indicator table, the manual condition mapping, and the ordinal-encoder output.
- [ ] **Check the order explicitly:** Verify that the intended condition progression is `Poor < Fair < Good < Excellent`, with codes increasing in that order.
- [ ] **Run a counterexample:** Change the explicit category order in a temporary experiment and explain why the codes change even though the observations do not.
- [ ] **Write an encoding decision:** For each column, state the chosen encoding and the meaning—or lack of meaning—of the resulting numbers.

## Completion criteria

- [ ] Department names use separate flags instead of being presented as a ranking.
- [ ] Condition order is explicitly supplied and matches its stated meaning.
- [ ] The manual mapping and `OrdinalEncoder` results agree for the same order.
- [ ] The explanation does not claim that ordinal codes imply equal gaps between condition levels.
- [ ] The tiny CSV is labeled invented practice data, not model-training data.

## Session notes

Add one short entry whenever you stop. Keep your own observations here; blank entries are prompts, not claims about work already completed.

### Session 1
- Date:
- Checkpoint worked on:
- What I observed or changed:
- Question to resolve:
- Next small step:

### Session 2
- Date:
- Checkpoint worked on:
- What I observed or changed:
- Question to resolve:
- Next small step:

### Session 3
- Date:
- Checkpoint worked on:
- What I observed or changed:
- Question to resolve:
- Next small step:

### Later sessions
Add another heading when you need one.

## Optional extension

Look up how an encoder can handle a category it did not see while fitting. Explain why that question matters when a model later receives new records; do not silently assign a new label an arbitrary rank.
