# To run Bluesky in Windows

1) Install Anaconda
2) configure shell (open anaconda shell  and type):
    conda init powershell

3) create the environment:

    - Anaconda GUI (python 3.10)
    - Anaconda shell: 
        conda create -n bluesky_win python=3.10 -y
    - Open VSCode and init the env: 
        conda activate bluesky_win
   

4) If Windows --> Install Microsoft Visual C++ 14.0 or greater is required
    - https://visualstudio.microsoft.com/visual-cpp-build-tools/

    - It is required this packages:
        - Desktop development with C++
        - MSVC v143
        - Windows 10/11 SDK
    

5) Upgrade build tooling

    pip install --upgrade pip setuptools wheel

6) Install known-good versions

    pip install numpy==1.23.5
    pip install scipy==1.10.1
    pip install pandas matplotlib
    pip install pygame==2.5.2
    pip install PyQt6 PyQt6-WebEngine
    pip install pyopengl msgpack pyzmq textual

7) Install Bluesky
    cd bluesky
    pip install -e .

8) Run Bluesky (and check the installation works)
    python BlueSky.py

    - It spents few minutes to start


