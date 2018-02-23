# Reintroducing Your Development Environment
## From projects to production-level code

### Guest lecture at General Assembly DC for the seventh Data Science Immersive Cohort

Outline:

- Overview

    - "Who even is this guy?"
    - Getting to know your computer
    - Projects to Production
    - AWS (time permitting)
    - Questions


- Who Even Is This Guy?

    - Bio
        - High School
            - Aerospace Engineering
            - Jazz Guitar
        - Virginia Commonwealth University
            - Political Science
            - Philosophy
        - Fairfax Hyundai and Kia
            - Customer Relations Manager
        - Center for the Study of Neuroeconomics at George Mason University
            - Research Fellow
            - PhD Student

    - What About Now?
        - General Assembly/Booz Allen Hamilton DataScience5k
        - Contract Work
            - MainStreet Bank
            - Rosy
            - ???
        - Research Interests:
            - Computer Vision
            - Adversarial Models
            - Hierarchical Memory Models
            - Neural Computing

Getting To Know Your Computer

    - The File System
        - Root vs. Home Directories
        - Finding a place for all your projects
        - Organization

    - Interacting with Terminal
        - Basic Commands
            - `cd`
            - `ls`, `ls -a`
            - `mv`
            - `cp`
        - vim

    - Editing Your `bash` profile
        - Customizing things so to make your life easier
        - aliasing (quick paths to desktop and jupyter notebooks)
        - formatting/prettifying (find link!)
        
    - Quick anaconda diatribe
        - I don't like anaconda...
        - Homebrew
        - xcode


How to turn your work into a deliverable

    - Project vs. Package
        - Projects are single purpose collections of code that should be easily run by an end user, no matter their level of technical expertise.
        - Packages are tools that can be integrated into other projects, and will be used by developers

    - Packages
        - Clone this project into your repo/ directory: [`cifar-extender`](https://www.github.com/messiest/cifar-extender)
      
    - cifar-extender
        - Structure
            - setup.py
            - requirements.txt
            - README.md
            - LICENSE.txt
            - <your-package>/
            - main.py/main.sh

     - setup.py
       - Provides an overview of your package, that is used for classification/tagging purposes
       
    - requirements.txt
        - A listing of the packages that are needed to run your code

     - README.md
        - A human-readable description of your package, and provides a description on its use

     - LICESNSE.txt
        - Provides legal protection for your work, and describes its appropriate use and reuse by others
        - [OSI](https://opensource.org/)
        - Common Licenses
            - BSD 2/3 Clause
            - MIT
            - Apache

    - <your-package>/
     - This is where you will put all of your code
     - Should contain the file `__init__.py`
     
     - main.py/demo.sh
        - this is the package level script that will execute your code

    - Projects
        - Clone this project into your repo/ directory: ['tf-retrainer'](https://www.github.com/messiest/tf-retrainer)
        
    - tf-retrainer
        - Project for retraining an Inception Net model on your own image data
        - Uses the TensorFlow transfer learning API
        - Allows you to create a custom image classification model

    - Computer Vision Digression
        - Algorithms for performing tasks with image data
        - Common tasks
            - Image classification
            - Object detection
        - Typically done with Convolutional Neural Networks
    
    - Transfer Learning Digression
        - The models that are trained are often incredibly deep, and are trained with massive datasets
        - Shameless Plug: [`cifar-image-classifier`](http://www.github.com/messiest/cifar-image-classifier)
        - Many of the complex features rely on the same fundamental features, so they can be used for a wide variety of tasks
        - Transfer learning enables you to retrain the final layers of a model to use the pre-trained knowledge

    - Running tf-retrainer
        - We'll run the transfer learning model on the images curated by `cifar-extender`

