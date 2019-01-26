### Some notes:

- It looks like you have references to both the react and blaze tutorials in here, I completed the blaze tutorial and did not have react installed so this branch attempts to get your form working according to the blaze instructions.

- To do this I:
    + ran `meteor remove kadira:flow-router kadira:blaze-layout static-html react-meteor-data`
    + ran `meteor npm remove react react-dom`
    + ran `meteor add blaze-html-templates reactive-dict` - you'll see these added to your .meteor/packages
    + removed the react references from client/main.js
    + ran `meteor remove autopublish` per the instructions from the tutorial
    + created a ui/body.js with some of the code from the blaze tutorial. This file is imported from client/main.js
    + you'll see that ui/body.js subscribes to tasks, and imports your ui/Task.js file, which I've updated with a skeleton of the blaze tutorial code. That is where you will put your 'click .toggle-checked', 'click .delete', and 'click .toggle-private' events from the tutorial.
    + moved all of the react tutorial code into a new directory: `react_tutorial_code`
    + ran `meteor reset` and then `meteor` was working fine


