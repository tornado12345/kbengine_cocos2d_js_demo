kbengine_cocos2d_js_demo
=============

## This client-project is written for KBEngine(a MMOG engine of server)

http://www.kbengine.org

## 中文

[Demo搭建文档](https://github.com/kbengine/kbengine_cocos2d_js_demo/blob/master/README_CN.md)，QQ交流群：461368412，[论坛](http://bbs.kbengine.org)

## Releases

	sources		: https://github.com/kbengine/kbengine_cocos2d_js_demo/releases/latest
	binarys		: https://sourceforge.net/projects/kbengine/files/


## KBE-Plugins docs

	https://github.com/kbengine/kbengine_js_plugins/blob/master/README.md


## Start:
	1. Download KBEngine(a MMOG engine of server):
		Download(KBEngine):
			https://github.com/kbengine/kbengine/releases/latest

		Build(KBEngine):
			http://kbengine.github.io/docs/build.html

		Installation(KBEngine):
			http://kbengine.github.io/docs/installation.html

	2. Use git to get the plugin(client) and demo-assets(server):

		In the kbengine_cocos2d_js_demo directory:

		* Git command: git submodule update --init --remote
![submodule_update1](http://kbengine.github.io/assets/img/screenshots/gitbash_submodule.png)

		* Or use TortoiseGit(menu): TortoiseGit -> Submodule Update:
![submodule_update2](http://kbengine.github.io/assets/img/screenshots/unity3d_plugins_submodule_update.jpg)

		* Or manually get the plugin(client) and demo-assets(server)

			Download plugin(client):
				https://github.com/kbengine/kbengine_js_plugins/releases/latest
				unzip and copy to "kbengine_cocos2d_js_demo/cocos2d-js-client/plugins/"
				(Note: the need to modify the folder name as "kbengine_js_plugins")

			Download demo-assets(server):
				https://github.com/kbengine/kbengine_demos_assets/releases/latest
				unzip and copy to "kbengine/"  (The root directory server engine, such as $KBE_ROOT)

	3. Copy "kbengine_cocos2d_js_demo\kbengine_demos_assets" to "kbengine\" root directory
![demo_configure](http://kbengine.github.io/assets/img/screenshots/demo_copy_kbengine.jpg)


## Configure Demo(Optional):

	Change the login address(Clear browser cache):

		kbengine_cocos2d_js_demo\cocos2d-js-client\main.js
			args.ip = "127.0.0.1";
			args.port = 20013;


## Start the Servers:

	Ensure that the "kbengine_cocos2d_js_demo\kbengine_demos_assets" has been copied to the "kbengine\" directory
		Reference：Start

	Check the startup status:
		If successful will find log "Components::process(): Found all the components!".
		Otherwise, please search the "ERROR" keyword in logs, according to the error description to try to solve.
		(More: http://kbengine.github.io/docs/startup_shutdown.html)

	Start server:
		Windows:
			kbengine\kbengine_demos_assets\start_server.bat

		Linux:
			kbengine\kbengine_demos_assets\start_server.sh

		(More: http://kbengine.github.io/docs/startup_shutdown.html)


## Start the Client:

	1. We simply use python to build web service
		Download and Install http://www.python.org/ftp/python/3.3.4/python-3.3.4.msi

	2. Excute the start_http_service.bat

	3. Enter the game
		http://127.0.0.1


## Screenshots:

![screenshots1](http://kbengine.github.io/assets/img/screenshots/cocos_js_demo1.jpg)
![screenshots2](http://kbengine.github.io/assets/img/screenshots/cocos_js_demo2.jpg)
![screenshots3](http://kbengine.github.io/assets/img/screenshots/cocos_js_demo3.jpg)
![screenshots4](http://kbengine.github.io/assets/img/screenshots/cocos_js_demo4.jpg)
