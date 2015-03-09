#### Some lessons and tips I've learnt so far at Founders & Coders from the amazing mentors and the holy internet.


## sudo! Super User Do

When you try to install applications, modules etc, you sometimes get asked to use the following example command
```
sudo install
```
Doing this will give the app/module access to all your files, which is a privacy issue. You should not have to do this most of the time. 

If you have installed something using *sudo*, you may want to reclaim ownership of your directory. To do this you need to run the following command:
```
sudo chown -R username [directory]
```

* npm example for [directory] ----> ~/.npm

In the future it would help to try and figure out the error rather than giving in to using sudo. 

### More info:
[Stack Overflow](http://stackoverflow.com/questions/16151018/npm-throws-error-without-sudo/16151707#16151707)

[Nelsonic](https://github.com/nelsonic)


--------
### General JS info:
A useful link to a wide range of JavaScript resources - Specially the *Reading* section:
[JS: The Right Way](http://jstherightway.org/#reading)

--------
### Node.js
A useful link to get started on making a server in [Node.js](http://blog.kevinchisholm.com/javascript/node-js/making-a-simple-http-server-with-node-js-part-ii/)


--------
### To run a quick server:

```
npm install node-http-server
```
Then when you need to run server run the following command:

```
http-server -p <port number>
```

--------

### React.js
A basic beginners tutorial for [React.js](https://scotch.io/tutorials/learning-react-getting-started-and-concepts), a front-end JavaScript library made by facebook.


-------
### Alternative to forking

IF you want to use a repo on github to then add to it without eventually pushing to it (as you would when you fork), then you have do the following: 

1. create an empty repo on github
2. clone the repo you want to copy (let's call this the parent repo)
3. cd into the parent repo and run the command:

```
git push --mirror https://github.com/USER/CHILD-REPO.git //mirroring only duplicates the repo but you are still connected to the parent, if you want to be separate from it do:
git remote set-url origin https://github.com/USER/CHILD-REPO.git
```
Now you can start working in the child repo. (This technique is useful for using starter kits to build your project on top of).
