# Getting Started: GitHub, Your Team Fork, and Google Colab

Complete this setup **before collecting laboratory data**. Every team uses one shared GitHub fork for the entire semester. Do not create one fork per student.

## What you are creating

- The instructor repository is `brash99/Phys201L`. Treat it as the source for released course materials.
- One student serves as the **repository manager** and creates the team's fork.
- The other team members join that same fork as collaborators.
- Everyone edits the same notebooks in the same team fork.
- Google Colab runs the notebooks; GitHub stores the team's official saved work.

## Before you begin

Have the following ready:

- access to your CNU email;
- a Google account that can use Google Colab;
- the names and GitHub usernames of every team member; and
- a decision about who will be the repository manager.

Only the repository manager performs Steps 2 and 3. Every team member performs Steps 1, 4, and 5.

## Step 1: Create and verify a GitHub account

If you already have a working GitHub account with a verified email address, sign in and continue to Step 2.

1. Go to <https://github.com/signup>.
2. Create a free personal account. Use a username you are comfortable sharing with your classmates and instructor.
3. Complete GitHub's email-verification message. GitHub restricts basic repository actions until the email address is verified.
4. Record your exact GitHub username and give it to the repository manager.
5. Recommended: enable two-factor authentication and save your recovery codes somewhere secure.

Official help: [Creating an account on GitHub](https://docs.github.com/en/account-and-profile/how-tos/account-management/creating-an-account-on-github)

## Step 2: Create exactly one team fork

The repository manager performs this step while signed in to GitHub.

1. Open the instructor repository: <https://github.com/brash99/Phys201L>.
2. Select **Fork** in the upper-right portion of the page.
3. On the **Create a new fork** page:
   - set **Owner** to the repository manager's personal GitHub account;
   - keep the repository name `Phys201L`;
   - keep **Copy the `main` branch only** selected, if that option appears; and
   - select **Create fork**.
4. Verify that the resulting page identifies the repository as `<repository-manager-username>/Phys201L` and says it was forked from `brash99/Phys201L`.
5. Copy the fork's web address and share it with every team member.

Stop if a team member has already created the team's fork. Use that existing fork rather than creating another one.

Official help: [Fork a repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo)

## Step 3: Invite every teammate to the shared fork

The repository manager performs this step from the **team fork**, not from `brash99/Phys201L`.

1. Open `<repository-manager-username>/Phys201L`.
2. Select **Settings**. If the tab is hidden, open the repository's tab menu and select **Settings**.
3. In the left sidebar, select **Collaborators** under **Access**.
4. Select **Add people**.
5. Search for a teammate's exact GitHub username and add that person.
6. Repeat until every teammate has been invited.

Only the repository owner can see the settings needed to send invitations.

Official help: [Inviting collaborators to a personal repository](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/repository-access-and-collaboration/inviting-collaborators-to-a-personal-repository)

## Step 4: Accept the collaborator invitation

Every invited teammate performs this step.

1. Sign in to the GitHub account whose username was invited.
2. Open the invitation from GitHub. Check both GitHub notifications and the email address associated with the account.
3. Select **Accept invitation**.
4. Open the team fork and confirm that its address is `<repository-manager-username>/Phys201L`.

Do not continue until every teammate can open the team fork. If Colab cannot find the fork later, an unaccepted invitation is a likely cause.

## Step 5: Complete the Colab save test

Perform this test before opening the Lab 1 notebook.

1. In the **team fork**, open `Start_Here.ipynb`.
2. Confirm the GitHub address belongs to the repository manager, not to `brash99` and not to another teammate.
3. Select **Open in Colab** if GitHub displays that option. If it does not, replace the GitHub portion of the notebook address with the following pattern:

   `https://colab.research.google.com/github/<repository-manager-username>/Phys201L/blob/main/Start_Here.ipynb`

4. Sign in to Google if prompted.
5. In Colab, edit the team-information prompts and run the test code cell.
6. Select **File -> Save a copy in GitHub**.
7. If prompted, authorize Colab to access GitHub. Confirm that you are authorizing the correct GitHub account.
8. In the save dialog:
   - choose `<repository-manager-username>/Phys201L`;
   - choose branch `main`;
   - keep the path `Start_Here.ipynb`;
   - enter the commit message `Complete Colab save test`; and
   - save the notebook.
9. Return to the team fork on GitHub and refresh the page.
10. Open `Start_Here.ipynb` and verify that the team names, code output, and new commit are visible.

The test is not complete until the saved changes are visible on GitHub.

## Step 6: Open and begin Lab 1

1. In the team fork, open `labs/Lab01_Density/Lab01_Density.ipynb`.
2. Confirm once more that the browser address belongs to the repository manager's fork.
3. Open the notebook in Colab.
4. Enter the team name and every team member's name at the top.
5. Immediately save a test commit back to the original path:

   `labs/Lab01_Density/Lab01_Density.ipynb`

6. Verify that commit on GitHub before entering substantial data.
7. Continue saving meaningful checkpoints during the laboratory period.

Do not rename the notebook, change its path, or save it into the instructor repository.

## Normal workflow for every laboratory

1. Begin from the team's shared fork.
2. Before opening a newly released lab, use **Sync fork -> Update branch** on GitHub.
3. Open the assigned notebook from its original path in the team fork.
4. Open it in Colab and verify every team member's name.
5. Save an early test commit.
6. Save additional checkpoints while working.
7. After the final save, refresh GitHub and inspect the official saved notebook.
8. The repository manager submits that notebook's GitHub URL through Scholar.
9. Each student separately submits the private individual effort report through Scholar.

## Common problems

### I cannot create a fork

- Confirm that you are signed in to GitHub.
- Confirm that your email address is verified.
- Check whether you have already forked `brash99/Phys201L`; if so, use the existing fork.

### I cannot see Settings or invite collaborators

- Only the owner of the team fork performs this task.
- Confirm that you are viewing `<repository-manager-username>/Phys201L`, not `brash99/Phys201L`.

### A teammate cannot edit or cannot see the fork in Colab

- Confirm that the exact GitHub username was invited.
- Confirm that the teammate accepted the invitation while signed in to that account.
- In Colab, confirm that the teammate authorized the same GitHub account.

### Colab wants to save to the wrong repository or creates another notebook

- Stop before saving.
- Select the team fork explicitly.
- Use branch `main` and the notebook's original path.
- Do not add `Copy of`, change the filename, or save to Google Drive as the team's official submission.

### GitHub reports a conflict when syncing or saving

- Stop and ask the instructor for help.
- Do not delete the repository, force an update, overwrite another student's changes, or create a replacement fork.

### My work appeared in Colab but not on GitHub

- A Colab runtime is not permanent storage.
- Use **File -> Save a copy in GitHub**, then confirm the commit on GitHub.
- If the commit is absent, the work has not been submitted to the team repository.

## Privacy

This repository and team forks are public. Never commit student ID numbers, grades, private feedback, completed individual effort reports, passwords, access tokens, or other sensitive information.
