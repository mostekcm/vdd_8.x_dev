# Patch for VDD

## Download

```bash
git clone git@github.com:/mostekcm/vdd_8.x_dev.git vdd_8.x_dev
```

## Post Install Steps

1.  Go to repo:

        ```bash
        cd vdd_8.x_dev
        ```

2.  Run Vagrant Up

        ```bash
        vagrant up
        ...
        ...
        ==> default: =============================================================
        ==> default: Install finished! Visit http://<some IP> in your browser.
        ==> default: =============================================================
        ```

2.  Install Drupal, follow instructions at `http://<some IP>`

## Usage
If you need extra help beyond the instructions at `http://<some IP>`, see the [VDD instructions](https://www.drupal.org/project/vdd).

## If doing Auth0 plugin development
For more detailed instructions see the [Auth0 Drupal README](https://github.com/auth0/auth0-drupal).

1.  Go to drupal modules director (drupal7 or drupal8):

        ```bash
        cd vdd_8_dev/data/drupal[7|8]/sites/all/modules
        ```

1.  Clone auth0-drupal

        ```bash
        git clone git@github.com:/auth0/auth0-drupal
        ```

1.  *drupal7 only* Switch to drupal7 branch

        ```bash
        cd auth0-drupal
        git checkout 1.x.x
        ```

1.  Enable and Configure the module by signing in as root and going to the modules page.
