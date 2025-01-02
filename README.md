# Pocillo-icon-theme-Snap

Unfortunately, you still need to use this command to theme installed Snap apps.
And reuse them when installing new Snap apps.

``` for i in $(snap connections | grep gtk-common-themes:gtk-3-themes | awk '{print $2}'); do sudo snap connect $i pocillo-icon-theme:icon-themes; done ```

The pocillo-icon-theme is now available on Snapcraft:

<a href="https://snapcraft.io/pocillo-icon-theme">
  <img alt="Get it from the Snap Store" src="https://snapcraft.io/en/dark/install.svg" />
</a>
