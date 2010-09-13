To utilize this profile, simply provide a drush_make stub file with the following content:

core = "7.x"
projects[] = "drupal"
projects[panels7][type] = "profile"
projects[panels7][download][type] = "git"
projects[panels7][download][url] = "git://github.com/EclipseGc/panels7.git"
