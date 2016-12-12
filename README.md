test
====

```
\
| .htaccess
| index.php		- instanciate lib\Router and passes all info it can get
|
├- \config				- ini and config files
|
├- \img				- graphics
|
├- \lib				- website objects
|	| Controller.php	- Core of the system - decides what to call and how to build
|	| Error.php	   	- Error and Exception handler (almost as mirror in operation of controller realize only 'gone-wrong' events)
|	| Model.php		- Service for ~Controller to communicate with DB
|	| Page.php		- operates with Template to get necessary elements and build it together
|	| JSON.php		- responds as echoing result
|	| Registry.php	- holds all data of application running
|	| Router.php		- 	digest details of request stores in Registry and calls Controller
|	| Template.php	- part of view - fetches elements from \view, fill with data
|	| View.php		- calls Page (OR other response type) to get result view
|	|
|	└- \base			- website objects abstract definitinons
|
├- \script				- javascripts
|
├- \style				- css
|
├- \view				- html re-uasable elements
|
└- \application		- apps
		├- \school		- school application
		├- \notes		- notes
```
