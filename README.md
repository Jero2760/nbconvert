Trying to use nbconvert inside Pressbooks to include Jupyter Notebooks in textbooks. In addition to show code, it is possible to access Github code as unique storage for the code

# nbconvert

## Installation

1. Install [WP Pusher](https://wppusher.com/) as a plugin in your Pressbooks site by downloading and installing the package from a zip file: go to your Pressbooks dashboard, Network Administrator, and select Plugins -> Add Plugins -> Upload Plugin. Upload your WP Pusher zip file, install it and activate it
2. Install the nbconvert plugin in your Pressbooks site: from the WP Pusher settings, add the nbconvert plugin by typing this uri into the git plugin installer: ghandic/nbconvert. Go to Network Administrator -> Plugins -> WP Pusher -> Install plugin -> [Repository host: select GitHub] -> [Plugin repository: type ghandic/nbconvert] -> Install plugin
3. Activate the nbconvert plugin for your network
4. Customize your book css as needed, since nbconvert.css from the plugin can require some adaptation (in your book go to Appearance -> Custom Styles -> Your Web Styles)

## How it works

Simply add a shortcode and a url to the notebook file into your page editor on wordpress and voila

`[nbconvert url="https://github.com/ghandic/confluenceapi/blob/master/examples/Updating%20a%20confluence%20page.ipynb"]`

PHP then sends the url to an nbviewer API that will convert the ipynb file to html

## Example of how it renders on Wordpress default theme

![](https://www.andrewchallis.co.uk/wp-content/uploads/2018/02/demo.png)
