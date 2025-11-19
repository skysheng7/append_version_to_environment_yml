# Appending version number in `environment.ymml`

Author: Sky Sheng

This repository contains a Python script that automatically adds version numbers to all conda and pip packages in your `environment.yml` file.

## How to use
1. Place this script in the same directory as your `environment.yml` file (e.g., `<my_folder_name>`)
2. Navigate to that directory in your terminal:
```
   cd <my_folder_name>
```
3. Run the script (replace `ai_env` with your environment name if different):
```
   python update_enviroment_yml.py --root_dir="." --env_name="ai_env"
```
