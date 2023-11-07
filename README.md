# github
Here are the issues I've had with GitHub so far for easy troubleshooting.

**1. Cloning a Repository:**
   - Clone a repository from a remote URL to your local machine.
   ```
   git clone <repository_url>
   ```

**2. Initializing a Repository:**
   - Create a new Git repository in your current directory.
   ```
   git init
   ```

**3. Checking Repository Status:**
   - View the status of your local repository, including untracked, modified, and staged files.
   ```
   git status
   ```

**4. Adding Changes to Staging Area:**
   - Stage changes for the next commit.
   ```
   git add <file(s)>
   ```

**5. Committing Changes:**
   - Create a new commit with staged changes and a commit message.
   ```
   git commit -m "Your commit message here"
   ```

**6. Pulling Changes:**
   - Fetch and merge changes from the remote repository into your local branch.
   ```
   git pull
   ```

**7. Pushing Changes:**
   - Push your local commits to the remote repository.
   ```
   git push
   ```

**8. Branching:**
   - Create a new branch or switch to an existing branch.
   ```
   git branch <branch_name>
   git checkout <branch_name>
   ```

**9. Merging Branches:**
   - Merge changes from one branch into another.
   ```
   git merge <branch_name>
   ```

**10. Creating a New Repository on GitHub:**
    - Create a new remote repository on GitHub.
    - You can do this through the GitHub web interface.

**11. Adding a Remote Repository:**
    - Add a remote repository URL to your local repository.
    ```
    git remote add <remote_name> <repository_url>
    ```

**12. Forking a Repository:**
    - Create a copy of someone else's repository on your GitHub account.
    - You can do this through the GitHub web interface.

**13. Pull Requests:**
    - Create a pull request to propose changes to a repository.
    - You can do this through the GitHub web interface.

**14. Reviewing Pull Requests:**
    - Review and comment on pull requests in a repository.
    - You can do this through the GitHub web interface.

**15. Issue Tracking:**
    - Create and manage issues to track tasks, bugs, and feature requests in a repository.
    - You can do this through the GitHub web interface.

**16. GitHub Pages:**
    - Host a website for your repository using GitHub Pages. You can use this to publish documentation or project websites.

**17. GitHub Actions:**
    - Set up and manage GitHub Actions workflows to automate tasks, tests, and deployments in your repository.

# Reset Data and New Setup
নির্দিত কমান্ডগুলি Git এবং GitHub রিপোজিটরি সাথে কাজ করার জন্য ব্যবহার করা হয়, তবে এই কমান্ড সমস্যায় পড়তে পারে এবং আপনার রিপোজিটরি ডেটা হারানোর আশঙ্কা আছে।

এই কমান্ডগুলি ব্যবহার করার আগে, আপনার রিপোজিটরির ডেটা এবং কনফিগারেশন ব্যবস্থাপনা নিশ্চিত করুন।

এই ধরণের কাজ করার আগে সতর্কতা সাবধান রেখে যান এবং ডেটা নুকশানের আশঙ্কা থাকলে আপনার ডেটা নিশ্চিত ভাবে ব্যাকআপ করুন।

যদি আপনি নিশ্চিত হন এই কমান্ড ব্যবহার করতে চান তবে রিপোজিটরি থেকে .git ডিরেক্টরি বিলাপ করার মাধ্যমে রিপোজিটরি পুরোনো করে নিন এবং একটি নতুন Git রিপোজিটরি সৃজন করুন:

1. `.git` ডিরেক্টরি বিলাপ করুন:
   ```
   rm -rf .git
   ```

2. একটি নতুন Git রিপোজিটরি সৃজন করুন:
   ```
   git init
   ```

3. সমস্ত ফাইলগুলি স্টেজ করুন:
   ```
   git add .
   ```

4. প্রথম কমিট সৃজন করুন:
   ```
   git commit -m "first commit"
   ```

5. মাস্টার ব্রাঞ্চ কে নতুন নাম দিন (যদি নিশ্চিত হন):
   ```
   git branch -M main
   ```

6. রিমোট রিপোজিটরির লিংক যোগ করুন:
   ```
   git remote add origin <আপনার-রিপোজিটরি-লিংক>
   ```

7. পুশ করুন:
   ```
   git push -u origin main -f
   ```

এই কমান্ডগুলি সতর্কতাসহ ব্যবহার করুন এবং সতর্কতা সাবধানী মেনে নিন, কারণ এই কমান্ডগুলি পুরোনো রিপোজিটরির ডেটা মুছে ফেলতে পারে এবং ডেটা পুনরুদ্ধার সম্ভাবনা নিয়ে অসুরক্ষিত করতে পারে।

# Branch Reset and Pulling Everything
1. ব্রাঞ্চ এর ডাটা ফেচ করুন:
   ```
   git fetch origin main
   ```
2. এবার ব্রাঞ্চ এর ডাটা রিসেট করার জন্য নিচের কমান্ডটি চালান:
   ```
   git reset --hard FETCH_HEAD
   ```
