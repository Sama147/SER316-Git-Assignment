Number Guessing Game

Branch Structure
- `main`: production branch.
- `dev`: branch for features.
- `feature1`: Experimental branch (merge conflict practice).
- `feature2`: Experimental branch (rebase practice).
- `feature3`: Experimental branch (squash practice).
- `hotfix`: Urgent fix for main.

## Branch Changes Description
- **feature1**: Adds encouraging messages for players.
- **feature2**: Implements maximum attempts logic and game over conditions.
- **feature3**: Adds a hint system to show proximity after 3 attempts.
- **hotfix**: Fixes `randomInt` to properly include the max value in its range.

## Learning Summary

### Merge vs. Rebase vs. Squash vs. Cherry-pick
- **Merge:** Combines two branches and creates a merge commit. It preserves the exact history of how branches diverged and joined. (Used in Step 2 & 6).
- **Rebase:** Moves a sequence of commits to a new base commit. It rewrites history to make it look like the feature was developed directly on top of the latest `dev` branch, keeping the history linear. (Used in Step 4).
- **Squash:** Combines multiple commits into a single commit. It is great for cleaning up messy "work in progress" commits before merging into a main branch. (Used in Step 5).
- **Cherry-pick:** Applies a single specific commit from one branch onto another. It is perfect for urgent hotfixes where you don't want to merge the entire branch. (Used in Step 7).

### Observations on Git History
- `feature1` and `feature2` showed how divergent histories can be brought together. `feature1` used a standard merge (creating a merge commit), while `feature2` was rebased to keep the history linear.
- `feature3` initially had 4 messy commits. After squashing and rebasing, it looked like a single, clean, professional commit on top of `dev`.