# MemoryLeakTopic

https://android-developers.googleblog.com/2009/01/avoiding-memory-leaks.html

https://medium.com/freenet-engineering/memory-leaks-in-android-identify-treat-and-avoid-d0b1233acc8

https://android.jlelse.eu/9-ways-to-avoid-memory-leaks-in-android-b6d81648e35e


Summary:
1. Context related:  Context from Activity and Application:
 >>> use the Application context instead of activity context;
2. Inter class and Anonymoue class:
 >>> Use static inner class 

A Open source libary for detecting memory leak
https://github.com/square/leakcanary
How it works?
 1) Create the instance with the application;
 2) Regiter the ActivityLifecycleCallbacks
 3) Rewrite the onActivityDestroyed
 4) Create a new refence by WeakReference of that Activity
 5) check the new reference is released or not...
 
 
