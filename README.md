# Kickstart Workshop

<<<<<<< Updated upstream
# Install Anaconda and Jupyter Notebook
=======
## Installation using GUI

### 1. Download Anaconda
![](/assets/1.png)

### 2. Accept the license by choosing `continue`
![](/assets/2.png)

### 3. Accept the license agreement
![](/assets/3.png)

### 4. Install anaconda
![](/assets/4.png)

![](/assets/5.png)

### 5. Complete installation
![](/assets/6.png)


## Using Anaconda navigator

### 1. Launch jupyter notebook from the navigator
![](/assets/7.png)

### 2. Create conda environment
![](/assets/8.png)


### 3. Open terminal to install packages
  ``` bash
    conda activate ml_kickstart
    conda install jupyter --yes
    pip install pandas numpy matplotlib 
    pip install scikit-learn opencv-python keras
```

[Reference](https://sparkbyexamples.com/python/install-anaconda-jupyter-notebook/)



# Alternate: Install Anaconda and Jupyter Notebook using the Terminal
>>>>>>> Stashed changes

1.   Download Anaconda    
        ```bash
        cd Downloads
        (For MacOS) 
        wget https://repo.anaconda.com/archive/Anaconda3-2022.05-MacOSX-x86_64.sh
        (For Linux)
        wget https://repo.anaconda.com/archive/Anaconda3-2022.05-Linux-x86_64.sh
        ```
2. Install anaconda using the bash script
    ```bash
    (For MacOS)
    bash ./Anaconda3-2022.05-MacOSX-x86_64.sh
    (For Linux)
    bash ./Anaconda3-2022.05-Linux-x86_64.sh
    ```
3. Press `Enter` to read the license agreement. Use `Space` to continue to the next page.
4. Enter `yes` to accept the terms of the license agreement.
5. Press `Enter` to install Anaconda to the default location.
6. Type `yes` to have Anaconda update your PATH.
7. You should see this message once installation is complete:
    ```
        Thank you for installing Anaconda!
    ```
8. Open a new terminal or enter the following command in your terminal:
    ```bash
    source ~/.bashrc
    ```
9. To verify it was installed, use this command:
    ```bash
    (base) username@ubuntu:~$ python --version
    ```

10. Create conda env
    ```bash
    conda create --name ml_kickstart python=3.8
    ```
11. Press `y` to proceed with env creation
12. You should see this message after successful conda env creation:
    ```bash
    # To activate this environment, use
    #
    #     $ conda activate ml_kickstart
    #
    # To deactivate an active environment, use
    #
    #     $ conda deactivate
    ```

13. Install packages:
    ``` bash
    conda activate ml_kickstart
    conda install jupyter --yes
    pip install pandas numpy matplotlib 
    pip install scikit-learn opencv-python keras
    ```

14. Running jupyter notebooks    
    ```bash
    cd <example_scripts_path> 
    jupyter notebook
    ```

15. Example output:
    ```
    (ml_kickstart) gautham@Ryuk-MacBook ml_kickstart % jupyter notebook
    [I 11:20:48.369 NotebookApp] Serving notebooks from local directory: /Users/gautham/src/ml_kickstart
    [I 11:20:48.370 NotebookApp] Jupyter Notebook 6.4.11 is running at:
    [I 11:20:48.370 NotebookApp] http://localhost:8888/?token=2c2010b4ae1f7777419692f0dce6adcee1986041381c2fea
    [I 11:20:48.370 NotebookApp]  or http://127.0.0.1:8888/?token=2c2010b4ae1f7777419692f0dce6adcee1986041381c2fea
    [I 11:20:48.370 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
    [C 11:20:48.405 NotebookApp] 
        
        To access the notebook, open this file in a browser:
            file:///Users/gautham/Library/Jupyter/runtime/nbserver-84782-open.html
        Or copy and paste one of these URLs:
            http://localhost:8888/?token=2c2010b4ae1f7777419692f0dce6adcee1986041381c2fea
        or http://127.0.0.1:8888/?token=2c2010b4ae1f7777419692f0dce6adcee1986041381c2fea

    ```

16. Access the notebook by copy pasting the URL listed in your terminal. For example, open your browser and search `http://localhost:8888/tree`