# AmazonAutomation
Page Object Model Selenium Framework Exercise for Amazon Website

1. Instructions on how to run the program

i. I've used nunit framework so the test can be run in visual studio 2015 or earlier version using nunit test adapter(3.4) nuget package.
ii. Test can also be run using nunit console application which a text base runner. You can also chose to run the program using nunit GUI which is a graphical runner.
iii. Test can also be run through team city or most build managment and contineous integration server applications.
IV. the test enviorment and the browser can be selected using AmazonTests config file.
V. Log4net is implemented to provide 'Steps to Replicate' in console output. This should help in investigation of failed tests. 
Vi. Page Object Model has been used for selenium automation framework.


2. Any assumptions and/or decisions you had to make during this assessment.

i. I made careful analytical assumption when selecting cetrain elements to validate if I arrived at the correct page. The assumption is that thoes elments are unique to that page. It would have been nice to be able to speak with developers to identify a unique tag/element belongs to each page.


3. Explain possible drawbacks or pitfalls in the solution provided

i. I am not a fan of explicit wait and I've used it at one place. I did explore other options such as wait for ajax, wait for page to load but still ended up using 3 sec explicit wait. I would love to have spend more time to come up with a solution which required no explicit wait.
ii. The tests can be run on IE but more work need to make the test compatible with IE driver.
iii. The latest version of selenium webdriver(2.53) has some issues with firefox browser. It requires more time to investigate and fix the issue.
