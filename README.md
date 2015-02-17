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

## More info:
[Stack Overflow](http://stackoverflow.com/questions/16151018/npm-throws-error-without-sudo/16151707#16151707)

[Nelsonic](https://github.com/nelsonic)
