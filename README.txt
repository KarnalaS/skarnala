Notes
***********************************
This is the Redux style of implementation for Field Development Platform. With
this, the application is having a single store with multiple states and the
states are being added and reduced on a need basis.

Configuration information are being loaded from an external file
`app.config.json`. This will help you to manage the deployments targeted to
environments such as Development, QA and Production

GENERAL
-------------------------------

The packages and build configurations on this application are maintained and
supported by the architecture team. Please report any issues you encounter to
the project package maintainers. If it turns out your issue is a bug in the
project implementation or cause problems in build pipeline itself, the
maintainers will report the issue upstream and resolve.

Please refrain from modifying the package contents in the project, as the call
graphs are threaded and depended.

To configure the application, you should have the following as a prerequisite

1. Code Editor (preferably Microsoft Visual Studio Code) -
   http://code.visualstudio.com/?wt.mc_id=DX_573435&utm_source=google&utm_medium=paid&utm_content=1&utm_campaign=Corp-FY16Q3March-Dev-PJVS&gclid=CN_Jw822wtECFecV0woduJ0N6A

2. Typescript version - 2.1.5 (To check typescript version, run tsc -v from
   command prompt)
3. Node - Version 4.5 or above (To check node version, run node -v from command
   prompt)
4. NPM – Version 3.0 or above (To check npm version, run npm -v from command
   prompt)

5. run npm install from command prompt
6. Copy and paste the `aloe` folder from _node_modules to node_modules folder.
   `aloe` is the short form for Angular Library for Enterprise.
7. Boiler plate for modules can be used, for building new modules. Please
   contact the project anchors.
8. To build the project in watch mode, use 'npm run server:dev'. This will run
   the application in localhost:3000


The build action may generate following folders in your application and these
folders and its contents are not permitted to push to git repo. Please don't
modify the contents of `.gitignore` files.

    a. node_modules (folder)
    b. dist (folder)
    c. dll (folder) 
    d. coverage

---------------------
Deployment Procedure
-----------------------
The production build (`npm run build:prod`) is readily deployable to servers
configured with Internet Information Services. Copy the contents of "dist"
folder to the targeted boxes, and make changes in `app.config.json` as per
requirements

For app development you may choose Google Chrome or Firefox.

Lastly, as a practice, test the application in Microsoft Internet Explorer ver
11.0 or higher, and please don't inject workarounds to meet functional
deadlines.

Happy Coding!!

<arun_sn@infosys.com>