# Reproduce

Setup

1. Download and setup
    1. pipenv install django
    2. pipenv install appmap
    3. python manage.py migrate
    4. pipenv shell

-------------

## Errors with self.subTest

1. Switch to branch `with-subtests`
2. run `APPMAP=true python manage.py test polls.tests.QuestionModelTests`
3. Note the error `AttributeError: type object '_SubTest' has no attribute 'test_was_published_recently_with_subtests [in the future]'`
