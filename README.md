Sculpin + Tailwind Landing Page Skeleton
========================================

This GitHub repository provides a skeleton implementation of a Sculpin
product or company landing page site using the Tailwind CSS library.

To view a demo of what the skeleton looks like by default, please visit
the GitHub demo page:

[https://beryllium.github.io/sculpin-tailwind-landing-skeleton/](https://beryllium.github.io/sculpin-tailwind-landing-skeleton/)

The repository is configured to be used as a "template repository", so
you can quickly get up and running with your own copy by clicking the
["Use This Template"](https://github.com/beryllium/sculpin-tailwind-landing-skeleton/generate)
button in the GitHub interface.

Alternatively, you can use Composer to create the project:

```
composer create-project beryllium/sculpin-tailwind-landing-skeleton my-blog
```

## Getting Up And Running

After cloning your generated template to your local disk, you'll need to
run some commands to get dependencies installed.

```
composer install
yarn install
```

Composer will require a working PHP installation. Yarn (or NPM) will
similarly require a working NodeJS installation.

## Customize Your Site

Once the dependencies are installed, the next step is to configure your
site and start the customization process.

1. Open the `app/config/sculpin_site.yml` file
1. Change the Title and Subtitle to match your desired blog name
1. Change the URL field to `url: ~` or `url: ''`, unless you plan on
   hosting your site on a subfolder of an existing domain. Subfolder
   hosting is currently demonstrated by the included configuration.
1. Optionally, set a google analytics ID or a Disqus shortname.
1. Modify (or remove) entries under the `social` heading to edit the
   sidebar.

After saving the file, you should now be able to generate the site:

```
vendor/bin/sculpin generate --watch --server
```

When this succeeds, it will attempt to host your website for local
previews at [http://localhost:8000](http://localhost:8000).

Any changes you make to the configuration or source files should trigger
a regeneration of the site, and a browser refresh will show the changes.

Using this self-hosted preview, you can tune your site before you look
to publish it elsewhere.

If you plan on using WebPack and Yarn to customize your CSS/JS/Tailwind
experience, the command to regenerate those files is:

```
yarn encore dev --watch
```

## Keep Up To Date

To be honest, I am not quite sure what the best way to do this is with
a template repository. It may actually be as annoying as applying new
changes by hand if you want your site to include them.

As a result, this template repository is fundamentally only a skeleton.
Once you clone the template, you are on your way to maintaining your own
customized Sculpin website.