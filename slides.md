
***

# meteor.js

***

# what is meteor.js

- fullstack javascript app framework 💪
- easy learning + [good documentation](https://www.meteor.com/install)
- rapid prototyping (insecure first)
- realtime default

***



# what is inside

- pure javascript 😻😻😍
- [ddp](https://www.meteor.com/ddp) "rest for websockets"
- reactive rendering
- mongodb [livequery](https://www.meteor.com/livequery)
- painless cordova mobile builds
- pages atmosphere

***

# architecture

![](assets/meteor-platform.png)

***

# install

- ```$ curl https://install.meteor.com/ | sh```
- then we haz `$ meteor`

> thats all - all you need is meteor

***

# create & run 🏃

- `$ meteor create leproject`
- `$ meteor`

=>

- minified & concatenated client
- nodejs server
- mongodb
- awsome dev enviroment
- [localhost:3000](http://localhost:3000)

***

# app structure

- `client`
- `server`
- `/public`
- `/private`
- `lib`

`if(Meteor.isClient)` `if(Meteor.isServer)` `if(Meteor.isCordova)`

***

# load order

- deepest directory
- 'lib' directory
- sorted by filename

***

# templates

- [spacebars](https://atmospherejs.com/meteor/spacebars) inspired by handlebars
- simple - no logic in templates
- compile to js

***

# ui interaction
- helpers
- events

***

# collections

```js
Yo = new Mongo.Collection('yos');
```

- insert|update|remove client & server
- optimistic ui with minimongo
- autopublish & insecure default

***

# security

> Q: how to make meteor secure?

> A: remove the insecure package

- publish & subscribe

***

# mvc with [iron:router](https://github.com/iron-meteor/iron-router)

`$ meteor add iron:router`

```js
Router.route('/', function () {
  this.render('Home', {data: {title: 'My Title'}});
});
```

***

# ideas

- routing
- model
- concat
- views
- seo page rendering
- oauth


- http://de.slideshare.net/scandiweb/meteor-presentation-42641921
- https://channikhabra.github.io/jschannel-meteor-talk/#/1
