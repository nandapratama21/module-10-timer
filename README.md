### Tutorial 10

**1.2. Understanding how it works.** 

![Screenshot2.png](screenshot/Screenshot2.png)

From the screenshot above, we can see that the async function
will be executed outside the main thread. The println!("Nanda's PC: hey hey"); statement in the main function is executed immediately after the async block is spawned. It does not wait for the async block to finish, hence "hey hey" can be printed before "howdy!" and "done!". 