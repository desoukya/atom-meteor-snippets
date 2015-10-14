# Meteor Snippets Package

[Meteor](https://www.meteor.com) snippets for [Atom](https://atom.io).  

### HMTL/Spacebars

| Snippet           | Output |
| :-------------    | :------------- |
| template          | ```<template name="$1">$2</template>``` |
| loginButtons      | ```{{> loginButtons}}``` |
| each              | ```{{#each $1}}$2{{/each}}```
| if                | ```{{if $1}}$2{{/if}}```

### Javascript

| Snippet           | Output |
| :-------------    | :------------- |
| helper            | ```Template.${1:name}.helpers({$2});``` |
| events            | ```Template.${1:name}.events({$2});``` |
| onRendered        | ```Template.${1:name}.onRendered(function ($2) {$3}); ``` |
| sessionSet        | ```Session.set('${1:key}', '${2:value}');``` |
| sessionGet        | ```Session.set('${1:key}', '${2:value}');``` |
| autorun           | ```Tracker.autorun(function ($1) {$2});``` |
| newCollection     | ```${1:Name} = new Mongo.Collection('${2:name}');``` |
| allow             | ```${1:Collection}.allow({$2});``` |
| allowEx           | ```${1:Collection}.allow({insert: function (userId, document) {$2}, update: function (userId, document, fieldNames, modifier) {}, remove: function (userId, document) {}});``` |
| deny              | ```${1:Collection}.deny({$2});```
| denyEx            | ```${1:Collection}.deny({insert: function (userId, document) {$2}, update: function (userId, document, fieldNames, modifier) {},remove: function (userId, document) {}});``` |
| user              | ```Meteor.user()``` |
| userId            | ```Meteor.userId()``` |
| methods           | ```Meteor.methods(function ($1) {$2}); ``` |
| call              | ```Meteor.call(${1:method}, ${2:arguents});``` |
| callAsync         | ```Meteor.call(${1:methodName}, ${2:arguments}, function (error, result) { if (error) {$3} else {}});``` |
| error             | ```new Meteor.Error('${1:error}', ${2:reason}, ${3:details});``` |
| Publish           | ```Meteor.publish('${1:name}', function () {$2});``` |
| Subscribe         | ```Meteor.subscribe('${1:publication}');``` |
| isClient          | ```Meteor.isClient``` |
| isServer          | ```Meteor.isServer``` |
