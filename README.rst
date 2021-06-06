=====
Polls
=====

Polls is a Django app to conduct Web-based polls. For each question,
visitors can choose between a fixed number of answers.

Detailed documentation is in the "docs" directory.

Quick start
-----------

0. Clone the project ::
    
    git clone https://github.com/a1723/django-polls && cd django-polls

1. Create and activate venv ::
    
    python -m venv env
    source env/bin/activate

2. Install requirements.txt ::
    
    pip install -r requirements.txt

3. Add "polls" to your INSTALLED_APPS settings like this ::

    INSTALLED_APPS = [
        ...
        'polls',
    ]

DON'T ADD polls to INSTALLED_APPS if you already have note is INSTALLED_APPS like: 'polls.apps.PollsConfig'

4. Include the polls URLconf in your project urls.py like this::

    path('polls/', include('polls.urls')),

5. Run ``python manage.py migrate`` to create the polls models.

6. Create new superuser ::

    python manage.py createsuperuser

4. Start the development server and visit http://127.0.0.1:8000/admin/
   to create a poll (you'll need the Admin app enabled).

5. Visit http://127.0.0.1:8000/polls/ to participate in the poll or http://127.0.0.1:8000/admin to admin the project.