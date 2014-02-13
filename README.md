twentytab-seo
=============


A django app that allows to manage the meta contents of pages. He needs twentytab-tree. It also allows to translate information related to pages

## Installation

Use the following command: <b><i>pip install twentytab-seo</i></b>

## Configuration

- settings.py

```py
INSTALLED_APPS = {
    ...,
    'mptt',
    'modeltranslation',
    'twentytab',
    'tree',
    'seo',
    ...
}
```

- urls.py

```py
urlpatterns = patterns('',
    ... ,
    (r'', include('tree.urls')),
    ...
)

```