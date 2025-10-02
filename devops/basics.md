# 🖥️ File System Commands (with Visual Examples)

## 📂 List & Navigation

```bash
pwd

output=>> /home/dipak/projects
```

```bash
ls

 Lists files/folders.

 output=>> 
 app/   notes.txt   server.js
```

```bash
ls -la

Lists all files including hidden ones in detailed format.

 output=>> 
 -rw-r--r--  1 user user   120 Sep  2 09:30 .env
drwxr-xr-x  2 user user  4096 Sep  2 09:31 app
-rw-r--r--  1 user user   200 Sep  2 09:32 server.js
```

```bash
cd app

Moves into `app` folder.

 output=>> 
 /home/dipak/projects/app
```



---

## 📁 Creating Directories

```bash
mkdir app

Creates a folder named `app`.

projects/
 └── app/
```

```bash
mkdir -p src/components

Creates nested folders in one go.


projects/
 └── src/
      └── components/
```


---


## 📄 Files

```bash
touch index.js

Creates an empty file.

src/
 └── index.js
```

```bash
cp index.js app.js

Copies a file.

src/
 ├── index.js
 └── app.js
```

```bash
mv app.js components/

Moves file to another folder.

src/
 ├── index.js
 └── components/
       └── app.js
```

```bash
rm app.js

Deletes file.

src/
 └── index.js
```

---

## 🔍 Viewing Content

```bash
cat index.js

Prints file content.

console.log("Hello World");
```

```bash
head -n 2 index.js
```
Shows first 2 lines.  

```bash
tail -n 2 index.js
```
Shows last 2 lines.  

---

## ⚡ Permissions

```bash
chmod +x script.sh

Makes `script.sh` executable.  


-rwxr-xr-x  script.sh
```

---

## 📦 Archives

```bash
tar -czvf project.tar.gz src/

Creates compressed archive.


project.tar.gz
```

```bash
tar -xzvf project.tar.gz

Extracts archive.  


src/
 └── index.js
```
