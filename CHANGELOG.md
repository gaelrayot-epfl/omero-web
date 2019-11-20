# 5.6.dev2 (October 2019)

## API Changes

 - OMERO.web now uses Django 1.11, upgraded from Django 1.8.
 - URLs must be referenced by `name` not path.to.view.method (previously
   some webgateway URLS lacked a name). For example, instead of
   `{% url 'webgateway.views.render_image' image_id theZ theT %}`, use
   `{% url 'webgateway_render_image' image_id theZ theT %}`.

# 5.6.dev1 (October 2019)

- First version of python3 support
- Focus on getting unit tests passing
- Instructions for dev installation

# 5.5.dev2 (August 2019)

- Improve README
- Add omeroweb.version
- Move templates to omeroweb/
- Bump to omero-py 5.5.1.dev1

# 5.5.dev1 (August 2019)

- Extract code from ome/openmicroscopy
- Make minimal changes for a functioning `python setup.py` (#1)