# streaming-01-getting-started

> Get started with Python for streaming analytics

Set yourself up for productivity and collaboration.
We assume no prior programming experience and that you want to 
get productive as quickly as possible.

## Prerequisites

1. Python 3.10 or higher
1. VS Code
1. VS Code Extension: Python
1. Git (configured)

Remember:

- **Spacing, Spelling, Capitalization**: With computers, these are critical. Always double-check!

---

## Verify Installations / Update Default Python

In VS Code, open a terminal window (View / Terminal).

```shell
git --version
python --version
python -m pip install --upgrade pip wheel
```

## Execute Utility Script (Diagnostics)

With your repo folder open in VS Code:

1. Click util_about.py.
1. If VS Code prompts, install the recommended Python extension.
1. Check the Python Interpreter: On the bottom-left status bar, you might see a version of Python indicated (e.g., Python 3.10.x).
1. If not, click on the bottom status bar where it should show the Python version or might say "Select Python Interpreter".
1. From the dropdown, choose your default Python version.
1. In VS Code, open a terminal window (View / Terminal).

```shell
python util_about.py
```
---


## Explore & Execute Project Scripts

With your repo folder open in VS Code, start exploring.
Open, read, and run each project script (each file will have a .py extension) in order.
You don't need to fully understand the code yet. 
Instead, try to figure out what each file is doing.

When you finish, you'll have an idea of some things possible using just the Python standard library. 
You'll have generated several new data files.
The streaming process will run continuously for quite a while. 
Read the comments in the file to learn how to stop the process.

In the terminal, if you need to re-run a command, you can simply press the up key until you find a command that you ran previously in the same terminal that needs to be run again.

## Update Edit README

Edit this README.md file. It uses Markdown, a simple and easy markup language.

- Keep the prerequisites and task headings. 
- Within the task headings, keep only the commands that worked on YOUR machine. 
- Remove unnecessary instructions once you've mastered them.
- Add any additional notes that will help you in the future.

## Sync to GitHub

Now it's time to get the local work you did on your machine, 
back up to your cloud repo in GitHub.


### Option A: Use VS Code (Easy!)

1. On the VS Code side panel, click the source control icon (look for a blue bubble with an number in it).
1. Important! Above the Commit button, it will say "Message". 
1. You MUST include a commit message. 
1. In the commit message input box, type "initial results".
1. Click the down arrow on the blue "Commit" button to "Commit and Push" to your GitHub repo. 

Verify: Open a browser to your GitHub repo and verify the files have appeared. 
In addition to the original files, you should have one or more new files and an edited Markdown file. 
If not, return to VS Code and edit/execute files as needed. 
Then commit and push again.

Common Issue: If your computer hangs because you forgot the commit message, 
just enter your message in the top line of the file it shows in the editor.
Then click the checkmark in the upper right to close that file and save your commit message.
"Sync your changes" to push to GitHub. 


I was able to commit using the Terminal in VS Code. Other than having to git add some files, there were no issues.

### Option B: Use Git Bash or Terminal Commands (Easy as well):

Open a new `Git Bash` or Terminal window. Run the following commands one at a time.
They will first add all the files (add "dot"). 
Then they will commit the changes with a message. 
Finally, they will push the changes up to GitHub.

```
git add .
git commit -m "initial results"
git push origin main
```


-----

## General Recommendations and Troubleshooting

The following are general recommendations and troubleshooting tips.

### Issue: VS Code - No Source Control Icon

Suggestion: If you're in VS Code, and you don't see the Source Control icon with a blue bubble, right-click on the sidebar icons, and make sure "Source Control" is checked.  

### Issue: VS Code wants to install an extension

If VS Code suggests an extension, it's often good to go ahead and try it. 
Do a search on the extension to learn more. VS Code suggestions are usually helpful. 

## Additional Resources

1. For more information about Git in VS Code, see [Using Git source control in VS Code](https://code.visualstudio.com/docs/sourcecontrol/overview).
1. For more information about editing Markdown in VS Code, see [Markdown and Visual Studio Code](https://code.visualstudio.com/docs/languages/markdown).


## Zach's Notes

Streaming data seems like an interesting way to pull in real time data from some source on the web. It can give us insights at a much faster rate than simply using a bounded data source. However, I can see there being some issues where there is too much data to make sense of, or newer data is always favored while older data is ignored, leading to some key insights being missed. The analytic potential of unbounded data is dependent on the nature of the data. For example, streaming in weather data every 15 minutes may lead somebody to believe that due to rising temperatures over a few day period in February, Spring is about to start and the cold weather and snow is no more. However, any midwesterner will know that a few nice days in the winter is not a good indicator that winter is almost over. Ignoring older data would lead to some poor results in this type of analysis.

Overall, this module went well. Even though I didn't know what all of the code did, it did not seem to matter, as the code was established enough that I could work backwards as needed to better understand the code or potential issues.