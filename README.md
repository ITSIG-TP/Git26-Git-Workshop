# 🌱 Git & GitHub Workshop

Welcome! 👋 This repository hosts all the materials for the **Git & GitHub Workshop**, conducted by the **Information Technology Student Interest Group (ITSIG)**.

Whether you have never touched a terminal before or just want to tidy up the basics, you are in the right place. By the end of this workshop, you will be comfortable with the everyday Git workflow that developers use all over the world.

## 📂 What's in This Repository

| Folder / File | Description |
|---|---|
| `Labsheets/` | The step-by-step lab sheet we follow during the session |
| `Materials/` | Practice files for the branching and merging exercise |


## ✏️ Exercise: Make Your First Pull Request

Want to practice contributing to a real repository? Add your name to our participant list and open a pull request. This is one of the most important skills for working on a team.

Here's the full workflow:

1. **Fork** this repository. Click the **Fork** button at the top right. This makes your own copy. Forking makes your own personal copy of someone else's repository on your GitHub account, so you can freely make changes without affecting the original.

2. Now that you have copied the repo with to your account, you can download the repo to your computer so you can start making changes. This is called cloning. **Clone your fork** to your computer:
```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

3. Link the original repo as upstream
This lets you pull in the latest changes from the workshop repo later. You only do this once.
```bash
git remote add upstream https://github.com/ITSIG-TP/Git26-Git-Workshop.git
git remote -v
```

4. Sync before you start (the safe habit)
Grab the newest version of `Participants.md` so you're working from the latest names. This is the step that prevents most conflicts.
```bash
git fetch upstream
git merge upstream/main
```

5. **Create a new branch**
Never work directly on main. Make a branch for your change:
```bash
git checkout -b add-my-name
```

6. **Make your edit**
Open `Participants.md` and add a line with your name, like this:
```
- Your Name (Your Diploma)
```

7. **Stage and commit**
```bash
git add Participants.md
git commit -m "Add <Your Name> to participants"
```

8. **Push** your branch to your fork:
```bash
git push origin add-my-name
```

7. **Open the pull request**
Go to your fork on GitHub, click **Compare & pull request**, write a short message, and submit. 🎉

That's it! You've just contributed to a shared project the same way professional developers do every day.


## 🙌 About ITSIG

This workshop is organised by the **Information Technology Student Interest Group (ITSIG)**. We run hands-on sessions to help students build practical tech skills and a supportive community.

Happy committing! 🚀
