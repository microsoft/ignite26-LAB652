@lab.Title

## What you will do

In this lab, you give a weekly job to Copilot Cowork. Cowork does the job and gives you the result. Then you make the job into a skill. You add a plugin, and you make Cowork do the job each week.

Time: 75 minutes. The last 5 minutes are for questions.

**Do not close this window.** If you close it, the lab ends. Minimize it if you need more space.

## Your sign-in details

You use these details to sign in to Microsoft 365:

- **User name**: +++@lab.CloudPortalCredential(User1).Username+++
- **Temporary Access Pass**: +++@lab.CloudPortalCredential(User1).AccessToken+++

> [!note] Text like +++this+++ is type text. Select it, and the lab types it for you.

## Words in this lab

| Word | Meaning |
|---|---|
| Cowork | A Copilot mode that does jobs with many steps for you. |
| Chat | The other Copilot mode. Chat answers questions. Cowork does jobs. |
| Task | One session with Cowork. Each task has a conversation, a side panel and files. |
| Side panel | The panel next to the conversation in a task. It shows the progress, the files and the skills. |
| Skill | Saved instructions that tell Cowork how you do a job. |
| Skill Report | A score from 0 to 100 that shows the quality of a skill. |
| Plugin | A package that adds skills and connectors to Cowork. |
| Connector | A connection that lets Cowork get information from a different service. |
| MCP server | A service that gives information to Cowork through a connector. |
| Automation | A prompt that Cowork runs again on a schedule. |
| Approval card | A small form in the task. Cowork uses it to ask you before it does an action. |

## Your story

You are a project lead at Contoso. Each Monday, you write a project status report. You read the project tracker and the meeting notes. Then you write the report and send it by email. The steps are the same each week, and the work is slow. You can also use this method for any weekly report.

===

# Exercise 0: Get ready (5 minutes)

### Open Cowork

1. [] Open the browser.
2. [] Go to +++https://copilot.cloud.microsoft/cowork+++.
3. [] Sign in with your **User name** and **Temporary Access Pass** from the first page of these instructions.
4. [] Make sure that you see a box where you can type a prompt.

> [!alert] If you see **Request access**, Cowork is not ready for your account. Ask a proctor. Do not select **Request access**.

### Put the lab files in OneDrive

1. [] Open a new browser tab.
2. [] Go to +++https://onedrive.cloud.microsoft+++. You are already signed in.
3. [] Select **Create or upload**, and then select **Files upload**.
4. [] Go to **Desktop** > **LAB652**.
5. [] Select these 2 files: **Project-Tracker.xlsx** and **Meeting-Notes.docx**. Select **Open**.
6. [] Wait until the upload is complete. You see the 2 files in **My files**.

You see Cowork in the first tab and the 2 files in OneDrive in the second tab.

> [!hint] If you do not see the **LAB652** folder on the desktop, ask a proctor.

===

# Exercise 1: Give a complex job to Cowork (15 minutes)

1. [] Go back to the Cowork tab.
2. [] Type this prompt:

    +++Make this week's project status report. Use Project-Tracker.xlsx and Meeting-Notes.docx in my OneDrive. Make the report a Word document with 3 parts: summary, status of each project, and risks. Then make an email draft to me with the report attached. Do not send the email.+++

3. [] Press **Enter**.
4. [] Read the steps that Cowork shows while it works. The side panel shows the progress.
5. [] Do not type while Cowork works. You can add messages, but for this lab, wait.
6. [] While you wait, read "About skills" at the end of this exercise.
7. [] When Cowork stops, find the status report in the side panel, in **Output folder**.
8. [] Open the status report.
9. [] Open Outlook in a new tab: +++https://outlook.cloud.microsoft+++. Find the email draft in **Drafts**.

You see a Word document with a summary, the status of each project, and the risks. You also see an email draft with the report attached.

> [!hint] If Cowork does not stop after 10 minutes, ask a proctor for the sample report.

> [!knowledge] **Key point:** Cowork made an email draft. It did not send the email. Cowork asks you before it sends an email.

**About skills:** a skill tells Cowork how you like to do a job. When you ask for that job again, Cowork uses the skill. You do not need to explain the steps again.

===

# Exercise 2: Make the process into a skill (15 minutes)

1. [] Go back to the Cowork tab. In the same task, type this prompt:

    +++Make a skill from the steps that you used for this status report. Name the skill weekly-status-report.+++

2. [] Press **Enter**.
3. [] Cowork asks you some questions. Use these answers:

    | If Cowork asks about | Type |
    |---|---|
    | Name | +++weekly-status-report+++ |
    | Description | +++Use this skill when I ask for the weekly project status report.+++ |
    | Category | +++Reports+++ |
    | Instructions | +++Use Project-Tracker.xlsx and Meeting-Notes.docx in my OneDrive. Write a short and clear report with a summary, the status of each project, and the risks. Always show late projects first. Never send the email.+++ |

    If Cowork asks other questions, answer in your own words.

4. [] Read the draft skill. Find the **Name** and the **Description**.
5. [] When the skill is correct, tell Cowork to save it. If Cowork shows an approval card, select **Approve**.
6. [] Read the **Skill Report**. Find the score from 0 to 100.
7. [] If the score is less than 70, ask Cowork to make the skill better. Do this a maximum of 2 times.
8. [] Start a new task.
9. [] Type this prompt, and press **Enter**:

    +++Make this week's project status report.+++

10. [] In the side panel, in **Skills**, find **weekly-status-report**.
11. [] Select **Customize**.
12. [] Select **Skills**. Find your skill in the list.

Cowork used your skill, and you did not type the skill name.

> [!hint] If Cowork does not use your skill, ask a proctor for the lab skill.

> [!knowledge] **Key point:** Cowork reads the **Description** to decide when to use a skill. Write in the **Description** when Cowork must use the skill.

===

# Exercise 3: Add a plugin (15 minutes)

1. [] Select **Customize**.
2. [] Select **Plugins**.
3. [] Select **Upload plugin**.
4. [] Go to **Desktop** > **LAB652**, and select the file **LAB652-plugin.zip**.
5. [] In the **Share** dialog, select **Only you**.
6. [] Select **Apply**.
7. [] Start a new task, so that Cowork finds the new plugin.
8. [] Type this prompt, and press **Enter**:

    +++Make this week's project status report. Add 1 tip from Microsoft Learn about how to write a good status report.+++

9. [] In the side panel, find the plugin name in **Skills**, or in the steps.

The status report has a tip from Microsoft Learn. Cowork used information that is not in your files.

> [!hint] If Cowork shows **Connect**, select **Connect**. You do not need to sign in. If you do not see the plugin, ask a proctor.

> [!knowledge] **Key point:** this plugin has 1 skill and 1 connector. The connector gets information from the Microsoft Learn MCP server. Your IT admin can make plugins available to all users in your organization.

===

# Exercise 4: Make an automation (10 minutes)

1. [] In the same task, type this prompt, and press **Enter**:

    +++Run the weekly status report every Monday at 09:00. Send the report to me by email.+++

2. [] Cowork shows the schedule. Make sure that the day is Monday and the time is 09:00.
3. [] Select **Activate and run now**. Cowork does the job 1 time now to test it.
4. [] Cowork shows an approval card to send the email. On the approval card, open **More options**.
5. [] Select **Only to** *your lab email address*.
6. [] Open your inbox. Find the email with the status report.
7. [] Go back to Cowork. Select **Automations**.
8. [] Select **Manage schedules**.
9. [] Find the automation for the weekly status report.
10. [] Select **Delete**. The automation will not run after the lab.

You received the status report by email. You know how to make Cowork do a job on a schedule.

> [!hint] If Cowork asks for approval again, select **Only to** *your lab email address* again. If this does not help, ask a proctor.

> [!knowledge] **Key point:** use **Activate and run now** to test an automation. Give your approval during the test. Your choice applies to this task. If Cowork asks again later, give your approval again.

===

# Exercise 5: Share the skill and find work for Cowork (10 minutes)

1. [] Select **Customize**.
2. [] Select **Skills**.
3. [] Select your skill **weekly-status-report**.
4. [] Select **Share**.
5. [] Select **Specific users in your organization**.
6. [] Optional: type the lab email address of a person near you.
7. [] Select **Apply**.
8. [] Copy the link in the **Share** dialog. You can send this link to the people that you shared the skill with.
9. [] Read the checklist below.
10. [] Think of 1 job from your work.
11. [] Use the checklist to decide if Cowork can do the job.

You shared a skill, and you know how to find work for Cowork.

> [!hint] If you cannot select **Share**, ask a proctor.

> [!knowledge] **Key point:** you can keep a skill for only you, or share it with specific people in your organization. If you change a shared skill, share it again.

### Checklist: is this a good job for Cowork?

1. Does the job have more than 3 steps?
2. Does the job use more than 1 file or app?
3. Is the information in Microsoft 365?
4. Can you describe a good result?
5. Do you do the job more than 1 time each month?
6. Can you check the result faster than you can do the job?
7. Is it easy to fix a mistake in the result?

If you answer "yes" 5 or more times, the job is a good job for Cowork.

===

# After the lab

You cannot copy files from the lab computer. To use the lab skill at work, do these steps:

1. Go to ++https://github.com/microsoft/ignite26-LAB652++.
2. Download the file **SKILL.md** from the **skills/weekly-status-report** folder.
3. In Cowork at your organization, select **Customize**.
4. Select **Skills**.
5. Select the arrow next to **Add**.
6. Select **Upload skill**.
7. Select the file **SKILL.md**.

You need a Microsoft 365 Copilot license to use Cowork. The people that you share skills with also need this license. Your IT admin must turn on Cowork.

Thank you for attending this lab.
