# marinebon_wordpress_website
This repo is for documentation and issue tracking as related to the main marinebon.org website as implemented using wordpress in 2022.

Web address: https://marinebon.org/

# NOTES:
## Main Menu Editing
The menu items are hard coded in file and WP admin section will not work for the menu. We have hard coded in file because the drop-down menu design is custom made and even if we allow it to update through the wp-admin section it will need little extra update and adjustment. A single misconfiguration while updating menu will mess up the whole menu and admin access and it can't be reverted immediately unless we fix it manually.

Here’s where you edit the menu manually (need to be logged in to admin): https://marinebon.org/wp-admin/theme-editor.php?file=theme-parts%2Fheader%2Fheader-menu.php&theme=labtechco

## Backups
* use “All in one WP migration” plugin and download a backup file.
* Login to the admin, and on the left side, look for All in one WP migration. 
* click “export” and select to save as a file.
* TODO: where do we keep these files?
* TODO: instructions for restoring

## Server spin up with Docker

Using `docker-compose.yml` per [wordpress - Official Image | Docker Hub](https://hub.docker.com/_/wordpress) with software versions [noted](https://docs.google.com/document/d/1nKsdq4Tvj06AnTzHWQAtd-z9UV8F37X3V4NyQmaWGA4/edit#bookmark=id.79kd52ao93gd):

```bash
docker compose up
```

### Restore from backups

* Using files uploaded by @7yl4r: [2022-11-22 | Powered by Box](https://app.box.com/folder/183228451933)
