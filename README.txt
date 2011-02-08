;To utilize this profile, simply provide a drush_make stub file with the following content:

api = 2
core = "7.x"
projects[drupal][type] = core
projects[drupal][version] = "7"

projects[panels7][type] = "profile"
projects[panels7][download][type] = "git"
projects[panels7][download][url] = http://github.com/EclipseGc/Panels-7.git
