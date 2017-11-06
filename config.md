## Export Config to File

In D8 you can export all of your sites configurations to yml files that can be put under version control.

The easiest way to do this is with the **Drupal Console**.
```bash
drupal config:export:content:type
```

This will ask 1. what module to save the content type's config in, and 2. what content type to export. 3. It will ask if the configuration should be optional or required.

Add the files to your modules version control, and then when you install the module on a different site, the content type will be created automatically with all of the corresponding fields. (**This only happens upon installation however**.)
