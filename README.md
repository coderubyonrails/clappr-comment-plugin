Clappr Comment plugin
==================

> A plugin for add comments and show comments on the seekbar of the Clappr HTML5 player

## Requirements

Clappr player: https://github.com/clappr/clappr

## Install

### Bower

```
$ bower install clappr-comment-plugin
```

### Git

```
$ git clone https://github.com/Metrakit/clappr-comment-plugin
```

### CDN (jsDelivr)

```
https://cdn.jsdelivr.net/clappr.comment/latest/comments.min.js
```

### Using the Plugin

Add both Clappr and Comments plugin scripts to your HTML:

```html
<head>
  <script type="text/javascript" src="http://cdn.clappr.io/latest/clappr.min.js"></script>
  <script type="text/javascript" src="dist/comments.min.js"></script>
  <!-- OR jsDelivr CDN -->
  <script type="text/javascript" src="https://cdn.jsdelivr.net/clappr.comment/latest/comments.min.js"></script>
</head>
```
Add the comments Plugin in the Clappr configuration
```javascript
      var player = new Clappr.Player({
        ...
        plugins: {
          core: [Comments]
        },
        ...
```

You can also add some options :
```javascript
      plugins: {
        core: [Comments]
      },

      // Comment options
      videoId: 1,
      urlGetComments: "http://localhost/comments-video",
      urlAddComments: "http://localhost/submit-comment",
      iconComment: "fa fa-comment-o",
      iconFont: "FontAwesome",
      pointerColor: "orange",
      enablePicture: true,
      texts: {
        addComment: 'Add a comment at',
        addCommentLink: "Comment",
        minutes: "minutes",
        commentPlaceholder: "Put a comment here",
        sendComment: "Send"
      }
```

### Options availables

- videoId : (integer) Id of the video
- urlGetComments : (string) the URL for get the comments
- urlAddComments : (string) the URL for add the comments
- iconComment : (string) the icon for add a comment
- iconFont : (string) the font for the icons
- pointerColor : the color of the cursors on the seekbar
- enablePicture : (boolean) availability to add pictures in the comments
- texts : multiple texts to translate

## Demo

http://labs.jordane.net/clappr-comment


## Author

- Metrakit (Jordane Jouffroy) : contact@jordane.net

## Credits

The Clappr Team : https://github.com/clappr/clappr/graphs/contributors
