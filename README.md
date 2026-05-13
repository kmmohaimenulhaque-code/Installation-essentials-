# Installation-essentials-
Install coding essentials from terminal 


On Ubuntu you don’t “hunt websites” for most coding tools — you install them from Terminal (recommended) or App Center (simple apps).

⸻

💻 Where to download everything

🧠 1. Python, Git, Node.js, build tools

👉 Download from Terminal (BEST way)

sudo apt update

Python

sudo apt install python3 python3-pip


📍Opencv is an externally managed environment. 

⸻

🧠 1. “externally-managed-environment”

Ubuntu is blocking system-wide pip installs to protect the OS.

So this is expected on newer Ubuntu versions.

⸻

🚀 BEST FIX (recommended)

Use a virtual environment (clean + proper way):

Step 1 — install venv support

sudo apt install python3-venv

⸻

Step 2 — create a project folder

mkdir opencv_project
cd opencv_project

⸻

Step 3 — create virtual environment

python3 -m venv venv

⸻

Step 4 — activate it

source venv/bin/activate

You’ll see:

(venv) username@ubuntu:~

⸻

Step 5 — NOW install OpenCV safely

pip install opencv-python opencv-contrib-python

No permission error now 👍

⸻

⚠️ About “permission denied”

If you also saw that, it’s usually because:

* you tried installing system-wide without sudo (blocked)
* OR Ubuntu protecting system Python

Never use sudo pip install (can break system Python 😭)

⸻

🧠 Simple rule

Action	Correct method
system tools	apt install
Python libraries	venv + pip
global pip install	avoid

⸻



Git

sudo apt install git

Build tools

sudo apt install build-essential

Node.js

sudo apt install nodejs npm

⸻

👁️ 2. OpenCV (VERY IMPORTANT for my personal project)

Not from App Center — from pip:

pip3 install opencv-python opencv-contrib-python

⸻

💻 3. VS Code (proper install)

Best way on Ubuntu:

sudo snap install code --classic

OR App Center → search:

Visual Studio Code

⸻



So you can ignore it here.

⸻

🌐 When DO you use browser downloads?

Only for things like:

* Blender
* Discord
* Chrome
* Zoom
* OBS Studio

Everything else = Terminal / App Center

⸻

🧠 Simple rule to remember

If it’s coding tools:

👉 Terminal (apt or pip)

If it’s big apps:

👉 App Center or official website

If it’s Python libraries:

👉 pip

⸻

🔥 Your clean setup path

Run this and you’re basically fully set:

sudo apt update
sudo apt install python3 python3-pip git build-essential
pip3 install opencv-python opencv-contrib-python
sudo snap install code --classic

⸻

