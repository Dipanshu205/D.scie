pandas help in data manipulation and data rangling 
it is a data manipulation library in python


example filtering a file data into new file --







Thanks for the update — this confirms your system is enforcing PEP 668 strictly, and even the --user flag is being blocked (which is unusual but now more common in recent Homebrew Python installs).

✅ Your safest and cleanest solution: Use a Virtual Environment
Let's do this step-by-step 👇

✅ Step 1: Create a Virtual Environment
In your pandas project folder (or any folder):

bash
Copy code
python3 -m venv venv
This creates a folder called venv/ containing your isolated Python environment.

✅ Step 2: Activate the Virtual Environment
bash
Copy code
source venv/bin/activate
Your terminal prompt will now show something like:

scss
Copy code
(venv) dipanshu@MacBook-Air pandas %
✅ Step 3: Install pandas inside the venv
bash
Copy code
pip install pandas
No errors this time — pandas will install here safely, without touching system Python.

✅ Step 4: Run Your Python File
Now run your Python file like normal:

bash
Copy code
python 01.py
(You’re inside the venv, so python here is the correct one.)

✅ Step 5: Deactivate when done

deactivate
This restores your normal shell environment.

🔁 Next Time You Come Back
Just run:

cd /path/to/your/project
source venv/bin/activate
and you're back in the clean Python environment, ready to run and install anything.