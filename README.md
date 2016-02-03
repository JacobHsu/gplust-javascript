# gplust-javascript

* [Quick-start sample app for JavaScript](https://developers.google.com/+/web/samples/javascript)  

```
git clone https://github.com/googleplus/gplus-quickstart-javascript.git
```

* https://developers.google.com/identity/sign-in/web/  

# console

https://console.developers.google.com/project/
 
憑證

OAuth 2.0 用戶端 ID  
Web client 1  

已授權的 JavaScript 來源  
http://jacobhsu.github.io  
已授權的重新導向 URI  
http://jacobhsu.github.io/gplust-javascript  

# gplus-quickstart-javascript.git

client:platform.js?onload=startApp  
startApp()  
gapi.load('auth2'  
gapi.client.load('plus','v1')  
gapi.signin2.render('signin-button'  
gapi.auth2.init( //console.log('init');  
updateSignIn() //console.log('update sign in state');  
auth2.isSignedIn.get() //console.log('signed in');  
helper.onSignInCallback(gapi.auth2.getAuthInstance());  
var helper = (function()  
onSignInCallback: function(authResult)  
authResult.isSignedIn.get()  
helper.profile()  
```
profile: function(){
      gapi.client.plus.people.get({
        'userId': 'me'
      }).then(function(res) {
        var profile = res.result; // console.log(profile);
```
>profile.image.url  
profile.displayName  
profile.aboutMe  
profile.emails  


