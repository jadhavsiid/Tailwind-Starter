# Tailwind-Starter
Commands to get started with Tailwind CSS

**Step-1:** Open a project folder/ working directory in an IDE.
<br>
<br>
**Step-2:** Inside that folder create two folders with names as- _**dist**_ (for production) and _**src**_ (for keeping code files), majority work we'll be doing in **dist**.
<br>
<br>
**Step-3:** Create **_index.html_** file inside **dist** folder.
<br>
<br>
**Step-4:** Open integrated terminal inside an IDE and type the following command:
```bash
#!/bin/bash
npx tailwindcss@3.4.3 init
```
this will create **_tailwind.config.js_** file in our working directory.
<br>
<br>
**Step-5:** Inside **_src_** file create a file named as- **_input.css_** , in which write following 3 lines in exact manner:
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```
> [!NOTE]
> It may show errors/problems due to linting, turn it off in settings.
<br>

**_Link this CSS file to the index.html created in an earlier step_**
<br>
<br>

**Step-6:** Inside **_tailwind.config.js_** file there would be an line beginning with **content: [ ]**, write:
```
content: ["./dist/*.html"];
```
this would target all the **_.html_** file getting rendered.
<br>
<br>

**Step-7:** Open integrated terminal and run the following command:
```bash
#!/bin/bash
npx tailwindcss@3.4.3 -i./src/input.css -o./dist/style.css --watch
```
<br>

**Congrats!!, You're ready to work with Tailwind CSS**
