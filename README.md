### Filestructure
 Use [sass globing](https://github.com/DennisBecker/grunt-sass-globbing) to pull in all the sass partials from the components directory. And we use [load-grunt-config](https://github.com/firstandthird/load-grunt-config) to seaprate the grunt file into individual files
```
 theme (custom theme) 
  | dev  
    - Gruntfile.js  
    - package.json  
    |- grunt  
	 - sass.js  
	 - sass-globbing.js  
	 - uglify.js  
	 - jshint.js  
	 - watch.js  
	 - aliases.yaml  
    |- node_modules (exclude from commits) 
    |- sass 
	 |- bourbon 
	 |- neat  
	 |- _custom.scss (main stylesheet)
	 |- _mixins.scss 
  |- components 
    |- custom_component (commit to github) 
	 |- php, scss and js files for the component 
    |- custom_component 
    |- custom_component 
```

### grunt modules we use
1. [uglify](https://github.com/gruntjs/grunt-contrib-uglify)
1. [sass](https://github.com/sindresorhus/grunt-sass) with [bourbon](http://bourbon.io/), [neat](http://neat.bourbon.io/)
1. [sass globing](https://github.com/DennisBecker/grunt-sass-globbing)
1. [load-grunt-config](https://github.com/firstandthird/load-grunt-config)
1. [watch](https://github.com/gruntjs/grunt-contrib-watch)
1. [jshint](https://github.com/gruntjs/grunt-contrib-jshint)
