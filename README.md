# meants
mean in typescript

Steps to setup:(follow up https://blog.logrocket.com/publishing-node-modules-typescript-es-modules/)
10) install git and tortoise git tool
20) download nodejs and install it. nodejs also include npm. Run "node -v" to verify it.
30) "npm install -g @angular/cli". run "ng --version" to verify it. 
40) "npm install -g typescript". run "tsc --version" to verify it

50) "ng new clientsample" to create angular client project
51) go to clientsample
52) run "npm install" to install dependencies.
53) run "ng build" to build
54) run "ng serve" to start serve
55) open browser and go to "http://localhost:4200" to see the client

60) make a serversample folder
70) go to serversample folder
80) "npm init -y" to create package.json
85） "npm install --save-dev typescript" to install typescript locallly
90) "npx tsc --init" to create tsconfig.json
120) for tsconfig.json:
	set target = ES2015, 
	module = es2015, 
	sourcemap = true
	outdir = "./dist"
	include = "./src"
130) for package.json
	set type=module
	main = "./dist/index.js"
140) for launch.json	
	set program = "${workspaceFolder}\\serversample\\dist\\index.js"
    sourcemap = true
    cwd = "${workspaceFolder}\\serversample".
	
150) npm install express
160) implement indexjs.js to serve angular JS. 

By this way to seperate the server and client totally. One server side may serve different clients such as web app client, phone client. 
