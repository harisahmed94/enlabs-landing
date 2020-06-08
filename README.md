# enlabs-landing

Here is the solution of the task. I am providing a brief documentation of this task for you to better understand the approaches which I took.

In terms of HTML, there is nothing special. Just used most of the components which are compatible with IE-11 and above. I used BEM so some of the HTML elements contain a lot of classes which is to be expected.

For CSS, I decided to use POST CSS because it is the fastest in terms of the computational times and supports some pretty neat features through plugins such as nesting, mixins, modularity, variables, auto-prefixing etc.

CSS file structure is organized as follows:
- styles.css (imports all the modules)
- base (containing global modules)
  - _global.css
  - _mixins.css
  - _typography.css
  - _variables.css
- modules (containing different blocks)
  - _call-to-action.css
  - _level.css
  - _progess-bar.css
  - _row.css
  - _section.css
  - _step.css
  - _wrapper.css
  
  Every block gets its own file containing styles related to its elements and modifiers in the "modules" sub-folder. This helps keep the code easier to manage and maintain. Used mobile first approach to make the site scale across a wide array of devices using the breakpoints specified in the description of the task.
  In terms of browser compatibility, everything should work well down to IE-11. Used webpack to bundle the files and to minify the CSS for the live version.
  
  PS: In my opinion, the background of the website could have been served better if the image and the gradient were on different layers in the PSD but I managed to work with it. I am not super happy with how it scales across different sizes but I guess that can be improved by making few adjustments from the designer.
