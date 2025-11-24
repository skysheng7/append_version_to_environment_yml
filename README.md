# Appending version number in `environment.ymml`

Author: Sky Sheng

This repository contains a Python script that automatically adds version numbers to all conda and pip packages in your `environment.yml` file.

## How to use
1. Place this script in the same directory as your `environment.yml` file (e.g., `<my_folder_name>`)
2. Navigate to that directory in your terminal:
```
   cd <my_folder_name>
```

3. Make sure you have installed `yaml` and `click` python packages. If you want, you can also use the `conda-lock.yml` file to recreate the environment I used to run the python script:

* Make sure you have installed `conda-lock`
* In your terminal, run: `conda-lock install --name <YOURENV> conda-lock.yml`. Please remember to replace `<YOURENV>` with the actual name of your new environment.
* Activate the conda environment: `conda activate <YOURENV>`

4. Run the script (replace `ai_env` with your environment name if different; replace `environment.yml` file name if you saved your package versions in a different file):
```
   python update_enviroment_yml.py --root_dir="." --env_name="ai_env" --yml_name="environment.yml"
```
