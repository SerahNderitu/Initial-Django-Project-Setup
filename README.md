# Initial-Django-Project-Setup


**Django** is a high-level Python web framework that enables developers to create dependable and scalable online applications quickly and effectively. 

With Django, developers can concentrate on writing the application logic while utilizing the framework's built-in tools for managing typical web development tasks, such as URL routing, database integration, user authentication, and template rendering.

Django is a well-liked option for developing sophisticated and feature-rich online applications because of its wide ecosystem of reusable parts and packages, emphasis on security, and scalability.

There are always a few setup procedures to finish before you can begin to construct the individual functionality of a new Django web application. This article serves as a guide for the procedures involved in setting up and managing a Django project.

To complete your Django project, you’ll need to have Python installed and understand how to work with virtual environments and Python’s package manager, pip. If you don't have much programming skills, don't worry because you won’t need much programming knowledge to complete this setup. However, in order to complete the initial Django project setup, you'll need to be familiar with Python.

## Starting a Django Project
Before starting a Django project, confirm that Python and Django are installed on your computer. If not, follow the instructions on [How To Effectively Install Django](https://github.com/SerahNderitu/Getting-Started-with-Django).

It’s advised to build Django projects in virtual environments. A virtual environment is a crucial tool for managing and isolating dependencies in a Django project. 

It allows developers to build a distinct environment with its own set of installed packages and Python interpreters, ensuring that the project's dependencies are consistent and do not conflict with other projects.

Developers can quickly manage and install packages tailored to their projects by using a virtual environment, facilitating effective collaboration and deployment. Read more to know how to get started with a virtual environment for Python.

If have already followed; how to get started with a virtual environment for Python, you have a virtual environment installed and activated in the location where you have your Django installation.

Your virtual environment's name, (env), will appear at the start of your command prompt if the activation is successful. Now you can go ahead and start a Django project.

To get started, run the following command;
```
(your-virtual-environment) $ django-admin startproject <your-project-name>
```

In this guide, we are going to use main as the name of the project. Therefore, the command will look like the following;
```
(env) $ django-admin startproject main
```

Running the above command, django-admin.py script is triggered to set up a new Django project by the name main. The command creates a directory with the project name and sets up the basic structure and configuration files for a Django project.

This command will create a directory named "main" in the current working directory and will contain all of the required files and directories for a Django project. Inside the "main" directory, you'll find files like "manage.py" (a command utility for administering Django projects) and a subdirectory with the same name as your project, which contains the project's settings and other configuration files.

Your default Django project can be illustrated as follows;
```
main/

     manage.py

    main/
      __init__.py
      settings.py
      urls.py
      wsgi.py
```

a. ``__init__.py``: The presence of the empty Python script __init__.py informs the Python interpreter that the directory is a Python package. This file enables the import of Python packages from the directories where they are located.

b. ``settings.py``: Contains the configuration settings for the Django project.

c. ``urls.py``: Contains URL patterns for the Django project.

d. ``wsgi.py``: Contains WSGI settings properties for the Django project. This Python script is used to support the operation of your development server and the release of your project into a production setting.

The **startproject** command will create projects with a similar structure.


## Running Your Django Project
After creating a Django project, we can now view it in action in the browser. For development, Django has a built-in web server. Run the command below while in the Base directory, which contains manage.py.We can now use the Django project we generated to check how it works in the browser.

For the time being, disregard all migration errors. Open your browser and navigate to http://127.0.0.1:8000/. If everything went according to plan, Django's default page should appear.


