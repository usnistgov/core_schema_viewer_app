Oxygen View Development Configuration
=====================================

Oxygen view instructions for development environment


1. Export the documentation from .xsd file using Oxygen
-------------------------------------------------------

Select the following format: *HTML output format*

- https://www.oxygenxml.com/doc/versions/20.1/ug-editor/topics/output-formats-documentation-XML-Schema.html#output-formats-documentation-XML-Schema__HTML-section


2. In your workspace under core_schema_viewer_app
-------------------------------------------------

Copy in core_schema_viewer_app/templates/core_schema_viewer_app/common/oxygen the following file:

    - am_schema_R2018a.html

Copy in core_schema_viewer_app/static/core_schema_viewer_app/common/oxygen:

    - am_schema_R2018a.html
    - docHtml.css
    - am_schema_R2018a_xsd.html
    - am_schema_R2018a.indexListns.html
    - am_schema_R2018a.indexListcomp.html
    - am_schema_R2018a.indexList.html
    - img folder


3. Start the server
-------------------

python manage.py runserver <port>


4. Connect to AMMD as administrator and upload the schema <your_schema>.xsd (here am_schema_R2018a.xsd)
-------------------------------------------------------------------------------------------------------

The Oxygen documentation view is now accessible at:

- <your_url>/schema_viewer/oxygen-viewer/<template_id>


EXTRA-NOTES
-----------

The name of the .html file have to be the same of the .xsd file (without extension)

- Here the xsd file name is:
          am_schema_R2018a.xsd

- The html file name is:
          am_schema_R2018a.html