# JoomGalleryPlugin
Content plugin for JoomGallery, a Joomla! component to maintain a photo library. This plugin allows to display single photos or photo galleries of a given category in Artlices and other pages on a Joomla! website.

This plugin is to a larger  reimplementation of the [JoomPlu](https://github.com/JoomGalleryfriends/JoomPlu) for Joomla! 4 and later. 

## Usage

The plugin relies on 'tags' that you insert in your Articles; tehse tags are replaced by HTML code to display a photo or category library. The syntax is:
```
{joomgallery:1 type=thumbnail}
{joomgallerycat:1 limit=12}
```
for a photo and a photo gallery respectively. The number after the colon is the id number of photo or category that you want to display. Several options can be specified; the options are seperated by a space from the id number.

### Photo options

 - type: image, original, thumbnail
 - align: left, right, center
 - float: 0 or 1: determines whether the figure floats, i.e. whether text can appear left or right of it (only works with left and right alignment)
 - linked: 0 or 1. When '1' (default), clicking on the picture will show the full size picture in a popup window.

Multiple options are separated by a pipe symbol '|'
```
{joomgallery:1 type=thumbnaili|align=right}
```

### Category options

 - columns: number of columns 
 - limit: max number of images to show

The defaults for these settings are given by the JoomGallery settings. 

JoomGallery is written and maintained by [JoomGalleryFriends](https://www.joomgalleryfriends.net/en/) ([github](https://github.com/JoomGalleryfriends/JoomGallery))
