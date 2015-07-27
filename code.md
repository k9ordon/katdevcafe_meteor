mongodb
127.0.0.1:3001








## helper & events

if (Meteor.isClient) {
  Template.hello.helpers({
    counter: function () {
        return 2;
    }
  });

  Template.hello.events({
    'click button': function () {
        alert('yo');
    }
  });
}














## mongo input

<template name="addform">
    <form>
        <input id="text"><button>go</button>
    </form>
</template>

<template name="history">
    History:
    {{#each messages}}
        <li>{{text}}</li>
    {{/each}}
</template>



Messages = new Mongo.Collection('messages');

Template.addform.events({
  'submit form': function (e) {
      e.preventDefault();
      Messages.insert({text: 'yolo'});
  }
});


Template.addform.events({
  'submit form': function (e) {
      e.preventDefault();
      Messages.insert({text: $('input').val()});
      $('input').val('');
  }
});


```

***

##

```js

```

***

##

```js

```
