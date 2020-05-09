#  Include Jupyter Notebooks in Pressbooks books

Pressbooks textbooks can now visualize Jupyter notebooks from GitHub repositories, making them accessible through GitHub and Google Colab as well. The Pressbooks book show the notebook code while it is maintained inside a GitHub repository. Readers can then go to interact and execute code without having to install anything locally. Authors can keep source code updated in just one place: the GitHub repo.

# nbconvert

## Installation

1. Install [WP Pusher](https://wppusher.com/) as a plugin in your Pressbooks site by downloading and installing the package from a zip file: go to your Pressbooks dashboard, Network Administrator, and select Plugins -> Add Plugins -> Upload Plugin. Upload your WP Pusher zip file, install it and activate it
2. Install the nbconvert plugin in your Pressbooks site: from the WP Pusher settings, add the nbconvert plugin by typing this uri into the git plugin installer: ghandic/nbconvert. Go to Network Administrator -> Plugins -> WP Pusher -> Install plugin -> [Repository host: select GitHub] -> [Plugin repository: type ghandic/nbconvert] -> Install plugin
3. Activate the nbconvert plugin for your network
4. Customize your book css as needed, since nbconvert.css from the plugin can require some adaptation (in your book go to Appearance -> Custom Styles -> Your Web Styles). My own Custom Styles file is [available here](https://github.com/Jero2760/nbconvert/blob/master/css/my_custom_styles.css)

## How it works

Simply add a shortcode and a url to the notebook file into your page editor on Pressbooks

`[nbconvert url="https://github.com/Jero2760/nbconvert/blob/master/example1.ipynb"]`

PHP then sends the url to an nbviewer API that will convert the ipynb file to html

## Example of how it renders on Pressbooks books

![](http://www.publiconsulting.com/wordpress/pythonfords/wp-content/uploads/sites/116/2020/05/demo.png)
