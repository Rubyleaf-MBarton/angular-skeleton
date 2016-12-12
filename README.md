Instructions
-------------

1. 'cd' to project folder and enter npm install && bower install in the terminal.
 
2. Navigate to node_modules/grunt-contrib-cssmin/tasks/cssmin.js and change line 41:
from - 
options.relativeTo = path.dirname(availableFiles[0]);
to -
options.relativeTo = path.dirname(availableFiles[0] || '');
This is due to an error being thrown otherwise about the string path not being specified.

3. Enter 'grunt' in the terminal.

4. Enter 'grunt serve' in a seperate terminal to run the application.

5. Enter 'grunt test' in the terminal to run the tests with karma.