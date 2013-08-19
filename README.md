# we_avatar

Choose an avatar image from your webcam or a file upload using HTML5 and jQuery

![](http://i.imgur.com/eAVDZwO.png) ![](http://i.imgur.com/7G7hvqt.png)

## Requirements

* jQuery
* [Twitter Bootstrap 2](http://getbootstrap.com/2.3.2/)
* Font-awesome (optional)

## Installation

### 1. Add we_avatar.js and we_avatar.css to your project.

### 2. Place this HTML where you want the image viewer/uploader to be:

    <div id="user_avatar" class="we_avatar centered_content" 
        data-mode="empty"
        data-image-url=""
        data-image-dataurl=""
        data-post-url=""
        data-delete-url=""
        style="width:160px; height:120px">
    </div>
    <div id="user_avatar_toolbar" class="we_avatar_toolbar"></div>

### 3. Setup the parameters:

* data-mode => "image" if there's already an image to show
* data-image-url => URL of the image to show
* data-image-dataurl => If you prefer, you can load the image in base64 here
* data-post-url => URL where the upload should be POSTed.
* data-delete-url => URL where a DELETE request will be made to delete the image.
* style => Size of the viewer/uploader

### 4. Fire the magic:

    <script type="text/javascript">
    jQuery(function(){
        we_start("user_avatar");
    })
    </script>

Note: Obviously you can change "user_avatar" to whatever you want.

### 5. Code the back-end side

*Rails example coming soon...*

---
## To-Do

* file upload -> RESIZED preview on canvas
* show post error/success
* CONFIG: button overlay texts & localized texts
* CONFIG: height and width (canvas & posted image)

