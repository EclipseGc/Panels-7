To utilize this profile, simply provide a drush_make stub file with the following content:

core = "7.x"
projects[drupal][type] = "core"
projects[drupal][download][type] = "git"
projects[drupal][download][url] = "http://github.com/drupal/drupal.git"

projects[drupal][patch][] = "http://drupal.org/files/issues/drupal.ajax_lazy_load_561858_142.patch"
projects[drupal][patch][] = "http://drupal.org/files/issues/850612-use-ajax-submit.patch"

projects[panels7][type] = "profile"
projects[panels7][download][type] = "git"
projects[panels7][download][url] = "http://github.com/EclipseGc/Panels-7.git"
