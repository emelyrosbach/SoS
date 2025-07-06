# Stuck on Suggestions: Automation Bias, the Anchoring Effect, and the Factors That Shape Them in Computational Pathology

## Overview

This repository provides the source code for the online experiment platform used in *"Stuck on Suggestions: Automation Bias, the Anchoring Effect, and the Factors That Shape Them in Computational Pathology."* We quantified automation and anchoring bias triggered by AI integration, and examined the additional roles of time constraints, professional experience, self-efficacy, and decision confidence during AI-supported evaluations. This was studied through a web-based experiment, where trained pathology experts (n = 28) estimated tumor cell percentages under various conditions.

## Contents

- **StudyPlatform:** The `StudyPlatform/` directory contains the Django project source code for the experiment interface, which participants used to rate tumor cell percentages. The `static/` subdirectory houses the study materials, including image patches from different H&E stained tissue slides (licensed under Creative Commons).

## Running the online experiment interface

1. Clone or download this repository and extract the files into a directory of your choice. Afterwards navigate to the `StudyPlatform/` subdirectory.

2. Make sure you have Python installed, then create a new virtual environment and install the `requirements.txt` file, e.g. with 
```
pip install -r requirements.txt
```
In VSC you may need to set/change the Python interpreter.

3. After running the follwoing commands you can access the experiment interface via http://127.0.0.1:8000/ or http://127.0.0.1:8000/XAI (for the AI-assisted version).
```
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
```

## License

The images located in the ```StudyPlatform/static``` directory were obtained with the necessary rights and modified (e.g., visualization of cell detections) to meet our specific requirements. As a result, we are able to publish these images for public use under the Creative Commons 4.0 BY-NC-SA License. Furthermore, the study user interface was designed using resources from Flaticon.com.
