This page shows a progress bar with the number of testers registered for the **STATIC Test Network**, that we hope will be up after the team have 512 testers or more.

You can see this page as a countdown, a way to inspire and keep interest from both new and old investors.

This page can later be modified for many other purposes.

External dependencies, with their own license:
 - https://xtrabytes.global/main.css
 - https://xtrabytes.global/xby_logo.png

# How to configure
The main configuration can be found in the `_config.yml` file, which has these items of most interest:
- `baseurl` must have the subdomain where this page will be hosted in, under the base domain defined
   in the `url` item. This must be configured.
- `testers_quantity_total` has the total number of testers required.
- `tester_line` and `tester_link` define both the text and the address of the
   link to the instruction to become a tester. This link is now shown if no more
   testers are required.

Progress bar is filled by the number stored in the file `_data/current_testers.yaml`, which must have the number of current registered testers.

A simple Ruby or Python script can be used to update the `current_testers.yaml` file and republish the static site using jekyll.