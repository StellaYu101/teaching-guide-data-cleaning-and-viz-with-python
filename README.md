# IRE/NICAR conference teaching guide for "Python: Data cleaning and visualization"

Thank you for volunteering to teach this one-hour session on using the `pandas` library to clean and visualize data. This teaching guide explains our setup and the material to cover.

The class is one hour long. The exercises live in [this Jupyter notebook](Data%20cleaning%20and%20visualization%20with%20pandas.ipynb).

It would be a good idea to [take a spin through the notebook](#run-the-notebook) prior to teaching the session.

## Session description
Now that you’ve got a handle on Pandas, it’s time to jump into some advanced topics. You know how to import a dataset, but what happens when you load the data and nothing looks right? We’ll walk through cleaning up a dirty dataset with Pandas. Then we’ll jump into the fun part: visualizing the data you’ve analyzed.

This session is good for: People who can load and perform basic summary and grouping functions in Pandas.

## Session goals
Attendees should leave with a basic understanding of:
- Grouping data
- Normalizing dirty data
- Renaming columns
- Creating new columns from existing columns
- Merging dataframes
- Visualizing data with bar charts and matplotlib
- Visualizing data with maps and geopandas

## Things you don't need to cover
- Anything related to virtual environments
- Things already covered in Python I and II

## General approach
I Do, We Do, You Do. Demonstrate a concept, go through it together, then give them plenty of time to experiment on their own while you and your coach walk around and answer questions (see sections marked `✍️ Try it yourself`). The pace will be slower than you think, and that's OK! It's not the end of the world if you don't get through everything.

Most people who come to this class will have _zero_ experience with programming, so be empathetic and try to remember how frustrating it is to feel lost.

## Class setup
We'll have the latest version of Python 3 and [pipenv](https://pipenv.readthedocs.io) to manage the virtual environment and dependencies (`jupyter` and `pandas`), which will already have been installed and tested prior to your session.

## Class outline

### Start up the notebook server
Begin the class by (slowly!) walking everyone through the process of activating their virtual environments and launching Jupyter:
1. Open Terminal (or `cmd` or `cygwin` if you're on a PC)
2. `cd` into your class directory
3. `pipenv shell`
4. `jupyter notebook`

It will take everyone a few minutes to get going. You'll also probably get some questions about what, exactly, you're doing at this step. Try to avoid a lengthy digression into virtual environments -- it's beyond the scope of this hourlong session, so maybe offer to talk to them after class, or send 'em our way: [training@ire.org](mailto:training@ire.org).

Once everyone is good to go, toggle back to the terminal and show them what's going on: A Jupyter server is running in the background, so don't close that terminal window!

Go over some notebook basics: Adding cells, writing code and running cells, etc. A common beginner gotcha: Writing code that other cells depend on but forgetting to first _run_ it to make it available.

### Main course content
Start marching down the 
notebook: Importing pandas, loading data from file, sorting, filtering, grouping. Pause frequently to ask if anyone has questions.

Any time you see `✍️ Try it yourself`, hit the brakes and give everyone time to play around with whatever concept you're discussing.

### Debugging
If you can, find an opportunity when someone has gotten an error and take 5 minutes to walk through basic debugging strategy: Reading the traceback error from bottom to top, strategic Googling, etc.

### If you have extra time at the end
Unlikely! But if you have extra time, oversee some unstructured lab time -- they can practice syntax or look up additional methods, etc.

### Ending the session
1. Have everyone close out of their notebook tabs
2. In terminal, `Ctrl+C` to kill the server process
3. Close the terminal window

## Run the notebook

You'll need the latest version of Python 3 and [pipenv](https://pipenv.readthedocs.io) installed on your computer. [Here's our install guide](https://docs.google.com/document/d/1cYmpfZEZ8r-09Q6Go917cKVcQk_d0P61gm0q8DAdIdg/edit?usp=sharing).

1. Clone or [download/unzip](https://github.com/ireapps/teaching-guide-intro-to-pandas/archive/master.zip) this repo onto your computer
2. In your command-line interface, `cd` into the folder
3. `pipenv install`
4. `pipenv shell`
5. `jupyter notebook`
