#Library Online Management System written in Django
---

####Link: http://django-library.herokuapp.com/

**Technologies**: django, python, html, css, less, Java Script, jQuery, Twitter Bootstrap, Git, Heroku, Selenium,
django_tables2, fandjango, Google App Engine (by CodeShip)

**Date**: December, 2014

>It is an online interface for a library (with a few social-network features) and allows users to:
- borrow/return books (like in real library) (a few real books are present in the system)
- create circles of friends (like in google+ or facebook) (add to friends and unfriend)
- share with friends books' quotation (in twitter style), borrowed books
- register/sign in via facebook and webpage
- save quotations from books

>There is also group of librarians with additional permissions:
- custom (outside of django admin) CRUD for authors, books' publishers, books etc.
- librarian can mark that book has been returned to library

Front-end is designed using Twitter Bootstrap and filled out with
sample data (mostly lorem ipsum). A few animations/effects are programmed using jQuery.

For facebook integration I used facepy and fandjango.

Application is provided with test (basic ones, unittests and selenium).

Data validations is done using (mostly) modelForms. 

Books/Authors/Publishers/Users search is made using django_tables2. It allows user to sort results
using selected criteria, watch selected amount of entries on page (pagination) etc. I have used user's images 
generated by gravator. 

**Exemplary system accounts**:

librarian account:
- login: assistant
- pass: 12345
- (do not worry, I have database backup ;))

standard user
- login: user1
- pass: 12345

I intended to document every fragment of code that could be unclear. Enclosed is documentation
created by sphinx.

**Run**: 
```sh 
python manage.py runserver 127.0.0.1:8888
```

(do not forget to change database settings if you want to run app locally) or simply **visit website: 
http://library-django.heroku.com/**

**Author: Tomasz Potanski, tomasz@potanski.pl**
