# strapi-hook-mongoose-bootstrap


This is fork from official strapi module.


This built-in hook allows you to use the [Mongoose ORM](http://mongoosejs.com/).

[Mongoose ORM](http://mongoosejs.com/) provides a straight-forward, schema-based solution to model your application data. It includes built-in type casting, validation, query building, business logic hooks and more, out of the box.

## Resources

- [MIT License](LICENSE.md)

## Links

- [Strapi website](http://strapi.io/)
- [Strapi community on Slack](http://slack.strapi.io)
- [Strapi news on Twitter](https://twitter.com/strapijs)

## Usage

Rename your model configs file located at 
  `{{project_folder}}/api/{{apiname}}/config/models`
  from `apiname.settings.json` to `apiname.settings.js`. 
  
  Add `module.exports` to export the config.
  
  Now you can add the function 
  ```
  boostrap: schema => {
   // stuff
  } 
  ```
  
I'll invoke before initializing moongoose model, therefore is useful to attaching mongoose plugins
