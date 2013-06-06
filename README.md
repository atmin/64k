64k
===

64k static webapp template
--------------------------


This project is currently in concept stage.


Goals
-----

* Python-based, self-contained, continuos build process (precompiles only what's changed)
* generate one self-contained HTML file (one request) per page, speedy to fetch even on high-latency networks (mobile friendly)
* use PJAX on modern browsers for lightning fast navigation after the single initial request
* load bare minimum, provide immediate feedback, load asynchronously non-critical parts
* built-in server
* Jinja2 templates, shape any site you want


Usage
-----

* `git clone https://github.com/atmin/64k.git my-app`
* `cd my-app`
* customize `_templates`
* customize `_data`
* start local server `./manage.py runserver`
* browse `http://localhost:6464`
* publish your changes `./manage.py publish`


Tasks
-----

* content organization
* JS framework
  * load `_data/*` files via PJAX
* Jinja2
  * custom tag to handle content namespace enumeration (generating index pages)

