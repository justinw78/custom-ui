# Custom-ui adapted
From Homeassistant version 110.+, icon handling has changed causing the original Custom-ui by @andrey-git no longer to be functional. Original repo at https://github.com/andrey-git/home-assistant-custom-ui

I've been a longtime and heavy user, and this is the place to applaud Andrey for his amazing plugin. Homeassisant wouldn't be the same without the global customizing it enables us to do. Couldn't live without it!
All credits go to Andrey.

This adapted version makes it compatible again with HA 110+.

Installing is super easy:

## Using Resources
-1 add a new folder under your resources folder. suggestion: custom-ui

-2 copy the custom-ui.js file to the folder

-3 add the following to your resources.yaml (adapt to your personal file hierarchy)
   ```yaml
   - url: /local/lovelace/resources/custom-ui/custom-ui.js?v=20200528
     type: module
  ```


## Using Frontend
If you don't use extra resources in Lovelace yet, you can also load the new custom-ui by changing you configuration.yaml as follows:
   ```yaml
   frontend:
     extra_module_url:
       - /local/lovelace/resources/custom-ui/custom-ui.js
   ```

-4 refresh the Lovelace resources

-5 refresh Lovelace


## Check the correct loading of Custom-ui
Having finished the above process,you should check if everything went well, and the info screens reflect the new adapted file as is should.

In `/developer-tools/info`
![info](https://github.com/Mariusthvdb/custom-ui/blob/master/Schermafbeelding%202020-05-28%20om%2012.31.07.png)

In Inspector
![inspector](https://github.com/Mariusthvdb/custom-ui/blob/master/Schermafbeelding%202020-05-28%20om%2012.31.51.png)

-6 happy customizing
