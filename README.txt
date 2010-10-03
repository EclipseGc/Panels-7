Currently working against the following issues:

Ajax Lazy Loading:
http://drupal.org/node/561858
Ajax Submission:
http://drupal.org/node/850612
Ajax insert commands:
http://drupal.org/node/736066
Ajax Options not Dynamic:
http://drupal.org/node/922796
Drupal initialize variable overrides of html errors:
http://drupal.org/node/917536

To utilize this profile, simply provide a drush_make stub file with the following content:

core = "7.x"
projects[drupal][type] = "core"
projects[drupal][download][type] = "git"
projects[drupal][download][url] = "http://github.com/drupal/drupal.git"

projects[drupal][patch][] = "http://drupal.org/files/issues/drupal.ajax_lazy_load_561858_180.patch"
projects[drupal][patch][] = "http://drupal.org/files/issues/drupal.ajax-use-submit.21.patch"
projects[drupal][patch][] = "http://drupal.org/files/issues/ajax-commandinsert-736066-30.patch"
projects[drupal][patch][] = "http://drupal.org/files/issues/922796-options-not-modifiable.patch"
projects[drupal][patch][] = "http://drupal.org/files/issues/allow_html_errors_in_php_ini.patch"

projects[panels7][type] = "profile"
projects[panels7][download][type] = "git"
projects[panels7][download][url] = "http://github.com/EclipseGc/Panels-7.git"
