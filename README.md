# Wagtail Admin Preview Tab

## Quick Start


1. Add `wagtail_admin_preview` to your `INSTALLED_APPS` settings file like this::

```python
    INSTALLED_APPS = [
        ...,
        'wagtail_admin_preview',
    ]
```
2. Start the development server and you will find the `preview` tab after the `content` tab in page editing view

## Purpose


The preview feature in wagtail admin requires you to open the page in another tab to preview.
This module simply adds another tab which shows you a preview of the latest draft saved without
requiring you to go open up another tab.

The default preview button is kept as is and the only addition is the preview tab so this has a
very minimal footprint on your project.

## Dependencies

This module requires:  
    1. Python >= 3.7 and  
    2. wagtail >= 3.0

## Configurations

You can configure the set of preview breakpoints by adding an array `WAGTAIL_ADMIN_PREVIEW_BREAKPOINTS` variable in your settings file.

*Please note that the breakpoints are only in pixels as of now. Future releases might support other units.* 

    ```python
    WAGTAIL_ADMIN_PREVIEW_BREAKPOINTS = [320, 528, 1366, 1920,4200]
    ```