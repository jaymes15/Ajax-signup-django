=====
ajaxsigniing
=====

ajaxsigniing is a simple Django app that helps to validate the username field in a sign up view, as soon as the user finish typing the desired username.

Detailed documentation is in the "docs" directory.

Quick start
-----------

1. Clone the repostoritory

2. change directory to cloned repo

3. Run `cd dist`

4. Run `dir` or `pwd` to get your current working directory you should see:
		 Directory of **:\**\**\**\django-ajaxsignup\dist          <<<<COPY YOUR WORKING DIRECTORY

11/28/2019  05:35 PM    <DIR>          .
11/28/2019  05:35 PM    <DIR>          ..
11/28/2019  05:35 PM             4,462 django-ajaxsignup-0.1.tar.gz
               1 File(s)          4,462 bytes
               2 Dir(s)  617,194,110,976 bytes free

5. open your application in the command,activate your virtual environment and RUN:
	    pip install <copied dir from step 4>\django-ajaxsignup-0.1.tar.gz
   i.e:    
		pip install **:\**\**\**\django-ajaxsignup\dist\django-ajaxsignup-0.1.tar.gz


6. Add "ajaxsigniing" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'ajaxsigniing',
    ]

7. Include the polls URLconf in your project urls.py like this::

    path('signup/',include('ajaxsigniing.urls')),

8. Run `python manage.py migrate` to create the ajaxsigniing models.

9. Start the development server and visit http://127.0.0.1:8000/signup/signup

TEMPLATE TAG USAGE
------------------

Add the below template tag to your signup template:

{% load custom_tags %}

{% sign_up  %}




