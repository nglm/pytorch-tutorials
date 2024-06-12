Installing Anaconda
===============================================================================

1. Install anaconda following the official instructions: [https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)
2. Open a terminal
3. Create an environment for the course by running the commands

    ```bash
    # List the versions of Python that are available to install
    conda search python
    # Create a "tuto" environment with the latest available version
    # of python (here 3.10)
    conda create -n tuto python=3.10 anaconda
    ```

   **Note:** While non-mandatory, working in a dedicated environment is highly recommanded. An environment is like an isolated "bubble" in your system, where you can (un)install whatever you need with anaconda, without any risk of conflicting with your actual system.

   - If something goes wrong in an environment (unlikely), you can simply delete the environment and recreate a new one. Your system won't be affected in any way.
   - With one environment per working task, you keep the number of dependencies in each environment low, which means lighter environments, with lesser risk of conflict between dependencies.

4. Activate the newly created environment by running the command ```conda activate tuto```

    **Note:** Once inside a given environment, installing a package with conda will automatically install inside the environment and nowhere else. In your terminal, you should see on the left ```(tuto)``` after activating your environment. Always make sure that you are in the desired environment before installing/running anything! When you're done working for this course, run the command '```conda deactivate```' to restore the terminal to the ```(base)``` environment (a default general purpose environment that is advised to keep as clean as possible by avoiding installing unnecessary things in it).

5. Install useful dependencies for this course (see the [installing_useful_packages_python.md](./installing_useful_packages_python.md) file)
