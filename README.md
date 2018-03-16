
### Component building 
1. Each component lives in its own file directory 
1. All js, php and scss files live in its own self contained component directory
1. Use css bem system for styling each component - this will ensure no component will conflict with another component

### Filestructure
 Use [sass globing](https://github.com/DennisBecker/grunt-sass-globbing) or similar to pull in all the sass partials from the components directory. 
```
 theme (custom theme) 
  |- components 
    |- custom_component (commit to github) 
	 |- php, scss and js files for the component 
    |- custom_component 
    |- custom_component 
  | dev  
    - Gruntfile.js  
    - package.json  
    |- grunt  
    |- node_modules (exclude from commits) 
    |- sass 
	 |- bourbon 
	 |- neat  
	 |- _custom.scss (main stylesheet)
	 |- _mixins.scss 
```
