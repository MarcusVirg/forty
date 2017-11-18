# Forty Theme

Forty theme is a multi page website built around a grid of image tiles that transition into its content pages. It is a ported theme built by [HTML5 UP](https://html5up.net/). This theme contains many styled elements and features a contact form. Built for blogs, businesses, or freelancers.

Insert screenshot here

## Installation

Create a new Hugo Site and inside the site folder run the following commands:

    $ cd themes
    $ git clone https://github.com/MarcusVirg/forty

To learn how to create a Hugo Site read the [official guide](//gohugo.io/overview/installing/) of Hugo.

### Netlify

If you are using Netlify to host your hugo site, you will want to add it as a submodule instead of cloning:

    $ cd themes
    $ git submodule add https://github.com/MarcusVirg/forty

This is because Netlify uses the hugo build command when autopublish is enabled and will produce an error if the theme is not a submodule. See the [Hugo Guide](https://gohugo.io/hosting-and-deployment/hosting-on-netlify/#use-hugo-themes-with-netlify) for more information.

## Using the theme

After cloning Forty or adding it as a submodule, there are a few other things you should do:

### Config File

There is an [`exampleSite`](//github.com/digitalcraftsman/hugo-agency-theme/tree/master/exampleSite) folder for this theme. Copy the file called [`config.toml`](//github.com/digitalcraftsman/hugo-agency-theme/blob/master/exampleSite/config.toml) to your websites root directory.
Here you can customize some of the text and content on the website.

### Change background

You can change the background by replacing the banner.jpg file with your own image in the folder forty/static/img. The image must be in jpg format and the filename must be called banner.jpg otherwise it will not work.

### Create new project/blog

To create a new blog post, you can take advantage of archetypes and use the Hugo command:

    $ cd hugoProjectDirectory
    $ hugo new blogs/myBlog.md

Replace `myBlog.md` with your own file name. You can also just copy the markdown files from forty/exampleSite/content/blogs

### Contact form

### Preview

You can see a preview of your site while developing it by running Hugo's built-in webserver.

    $ hugo server -D

Now enter [`localhost:1313`](http://localhost:1313/) in the address bar of your browser to see your site.

`NOTE: In the command above -D loads content that is marked as a draft. You can switch content from draft to final by changing the frontmatter value of draft to false in the .md file for the content.`

## License

This theme is released under the Creative Commons Attribution 3.0.
For more information read the [License](//github.com/digitalcraftsman/hugo-agency-theme/blob/master/LICENSE).

## Acknowledgements

Thanks to:

- AJ from [HTML5 UP](https://html5up.net/) for creating the theme
- [Steve Francia](//github.com/spf13) and [digitalcraftsman](//github.com/digitalcraftsman) for creating and maintaining Hugo.