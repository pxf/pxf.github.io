---
title: Getting Started
layout: support
categories: support
---

Getting Started
===============

Installation
------------
* ### Installation
	
	In the current version, the program will extract everything related to the plugin in the same directory as the program is started in.

	Directory layout:
	* `export/` - Scene export plugin for Maya
	* `plugin/` - Bake plugin for Maya
	* `samples/` - Baking sample scenes
	* `support/` - Misc


* ### Reinstallation
	Remove the `install_lock` file and start the `pxfplugin.exe` again.

* ### Updates

	PXFPlugin will automatically check for updates when started.


Setting up the scene
--------------------
1. ### Adding bake cameras
	TODO

2. ### Configuring PXFBake
	Before the scene can be baked, make sure the bake settings has been setup correctly. To open the configuration
	dialog, locate and press the configuration button in the PXFBake Plugin Toolbar.
	![Configure button](/static/help_config_button.png)

	![Configuration Overview](/static/help_config_overview.png)
	* Project
		* `Output directory` - Specify where on the disk to save scene, HTML files and bake textures.
		* `Create HTML project` - If checked, will generate a default HTML page that loads and bakes the scene.
		* `Filetype` - What image format the camera outputs should be saved as.
	* Render - (These are options passed directly to the Maxwell renderer.)
		* `Render Time` - 
		* `Sampling level` - 
		* `Render width` - 
		* `Render height` - 
		* `Number of threads` - 
		* `Write MXI` - 
	* Advanced
		* `Render filenames` - 
	* General
		* `Debug` - 


	**NOTE:** `Output directory` can be set to `./`, but in the current version of the plugin the render thumbnails may not appear.

	**NOTE:** Make sure to save the settings before baking the scene.

Baking
------
1. ### Start baking
	To start a scene baking, press the Bake All button located in the PXFBake Plugin Toolbar.

	![Bake All button](/static/help_bakeall_button.png)

	A bake progress window will appear when the scene has started baking/rendering.
	![Bake All overview](/static/help_bakeall_overview.png)

	When the bake process has finished, a tiny web server will spawn and the default browser will automatically open the newly created 3D scene.

Troubleshooting
---------------
TODO