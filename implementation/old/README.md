####This is just an old implemetation put here as proof of concept

*I've been using this for years without issues and think it's now time to share, and even make a better version it*

This version works perfectly fine, but does not support recursion like the posted spec proposes, and in ajax intensive sites you should see +40% bandwidth gains at least as far as ajax centric traffic is concerned.

####If you build a client or server-side implementation that supports the JsonR Spec, please submit it to the project

1. Clone the project
2. Add your implementation
3. Issue a pull request
4. Smile !



####Usage:

1. Add jsonr.js to your HTML page
2. Configure your project so that the string result from GetUsers() is returned to your browser client

Which should return:

    {"Values":[["Robert",41],["Teddy",35]],"Keys":["Pseudo","Age"]}


Then call merge() while passing it your result.

Now you should have:

    [{"Age":31,"Pseudo":"Robert"},{"Age":45,"Pseudo":"Bob"}]


####Note:
In this implementation size savings only start to kick in when you are dealing with collections containing more than 2 items