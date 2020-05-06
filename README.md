Trying to use nbconvert inside Pressbooks to include Jupyter Notebooks in textbooks. In addition to show code, it is possible to access Github code as unique storage for the code

# nbconvert

## Installation

1. Install [WP Pusher](https://wppusher.com/) by downloading and installing the package from a zip file 
2. From the WP Pusher settings, add the nbconvert plugin by typing this uri into the git plugin installer: ghandic/nbconvert
3. Activate the nbconvert plugin for the network

## How it works

Simply add a shortcode and a url to the notebook file into your page editor on wordpress and voila

`[nbconvert url="https://github.com/ghandic/confluenceapi/blob/master/examples/Updating%20a%20confluence%20page.ipynb"]`

PHP then sends the url to an nbviewer API that will convert the ipynb file to html

## Example of how it renders on Wordpress default theme

![](https://www.andrewchallis.co.uk/wp-content/uploads/2018/02/demo.png)
