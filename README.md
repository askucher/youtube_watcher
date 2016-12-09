# youtube_watcher
Watch youtube comments and posts and answer from your neural network


![youtube](https://i.ytimg.com/vi/s5y-4EpmfRQ/maxresdefault.jpg)

Install 
```javascript
npm install flyber_youtube_watcher
```

Use in your code
```javascript

var youtube_watcher = require("youtube_watcher");

var youtube_user = require("youtube_watcher/user");

var you = youtube_user({byLogin: "yourLogin", password: "password"});

var subscription = youtube_watcher.subscribe( {byFilter: "football"} );

subscription.on("upload", function(upload) {

    var text = upload.text;
    
    //apply your code here
    
    you.reply(upload, "your Comment");

});


subscription.on("comment", function(comment) {

    var text = comment.text;
    
    var uploadText = comment.upload.text;
    
    //apply your code here
    
    you.reply(upload, "your Comment For Post");
    
    you.reply(comment, "your Comment For Comment");

});



```

In order to get this working please contact to a.stegno@gmail.com

```Price
Subscription: 50$ per month. 
```

The website http://flyber.net

