To quickly add settings to all sites running through this deployment of
buildkit, simply create a *.php file in a suitable directory.

The following directories will be scanned (listed from highest to lowest
priority):

  $SITE_DIR/wp-config.d
  /etc/wp-config.d
  $PRJDIR/app/config/$TYPE/wp-config.d
  $PRJDIR/app/wp-config.d

If the same file appears in multiple directories, it will only be loaded
from the directory with highest priority.

For more advanced logic, one can look at global $civibuild or at any of the
standard CiviCRM configuration directives.

Files which end in *.php.ex are examples which can be copied.