sol
===<!DOCTYPE html>
<html>
  <head>
    <title>Contact Example</title>

    <script type="text/javascript" charset="utf-8" src="cordova-x.x.x.js"></script>
    <script type="text/javascript" charset="utf-8">

    // Wait for Cordova to load
    //
    document.addEventListener("deviceready", onDeviceReady, false);

    // Cordova is ready
    //
    function onDeviceReady() {
        var myContact = navigator.contacts.create({"displayName": "Test User"});
        myContact.note = "This contact has a note.";
        console.log("The contact, " + myContact.displayName + ", note: " + myContact.note);
    }


    </script>
  </head>
  <body>
    <h1>Example</h1>
    <p>Create Contact</p>
  </body>
</html>
