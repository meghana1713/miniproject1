1)
npm install -D tailwindcss is a command used to install the Tailwind CSS library as a development dependency in a Node.js project which can be seen in package.json file (this file will be created after we run npm install -D tailwindcss  command) this libraries will install in developemt stage  when we send to production this tools or libraries will not install
 {
  "devDependencies": {
    "tailwindcss": "^3.4.11" //devDependencies means at developement stage whatever tools like libraries  we install them and can be seen in this object in package.json file
  }
}
2)npx tailwindcss init:-
Creates a tailwind.config.js file, which allows you to customize Tailwind's default settings (e.g., adding custom colors, fonts, etc.).

3)npm init -y:
Running npm init -y in your project directory will create a package.json file that looks something like this:
in package.json 
{
  "name": "my-project",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {},
  "author": "",
  "license": "ISC"
}
-----------------------------------------------------
4)"watch": "npx tailwindcss -i ./src/input.css -o ./src/output.css --watch":-
npx tailwindcss: This command runs the Tailwind CSS CLI tool.(i.e in place of src we can keep./ as it is current folder)
-i ./src/input.css: Specifies the input CSS file.
-o ./src/output.css: Specifies the output CSS file.
Starts Tailwind CSS: It runs a command to process your CSS.
Watches for Changes: The --watch part means it keeps running in the background.
Rebuilds Automatically: Whenever you make changes to input.css or related files, it updates output.css automatically.
-------------------------------------------------------
5)  "build":"npx tailwindcss -i ./input.css -o ./output.css"
in "scripts" section in your package.json defines custom npm commands that you can run with npm run <script-name>
 the custome npm commansds are 1)"watch": "npx tailwindcss -i ./src/input.css -o ./src/output.css --watch"
 2)

npm run watch: Keeps an eye on your input  files and updates output.css automatically as you work.
npm run build: Creates  output.css one time, with no continuous monitoring
-------------------------------------------------------------------------
IF WE DEVELOPE CSS IN TAILWIND THEN WILL SENDING TO PRODUCTION WE NEED TO CHANGE THEM IN TO NORMAL CSS BY USING ALLTHE  5 steps
