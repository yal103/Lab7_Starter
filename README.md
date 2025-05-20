# Lab 7

1) Where would you fit your automated tests in your Recipe project development pipeline? Select one of the following and explain why.

    a. Within a Github action that runs whenever code is pushed

    b. Manually run them locally before pushing code

    c. Run them all after all development is completed

    > I would fit my automated tests in the Recipe project development pipeline **within a Github action that runs whenever code is pushed**. This is because it ensures that every push that is made to a repository does not break the code. After each change, it ensures that the interactions with the localStorage, rendering, and component integration work as expected. For example, any change to `RecipeCard.js` or `main.js` could break the code (ex. rendering, event listeners, form behavior). Manually running tests locally before pushing code is less ideal because it is not enforced, it is inconsistent, and easy to forget. Running the tests after all development is complete is also not ideal before it will be very hard to find the bugs and issues in the code.

2) Would you use an end to end test to check if a function is returning the correct output? (yes/no)

    > **No**, unit tests are more ideal.

3) What is the difference between navigation and snapshot mode?

    > Both Navigation mode and Snapshot mode in Lighthouse analyzes the performance, accessibility, best practices, and SEO of a web page. However, Navigation mode is determines these metrics based on a single page load while Snapshot mode is based on the current state of the page without reloading. Navigation mode is more ideal for testing the overall performance of the web page while Snapshot mode is more ideal for finding accessibility issues in the throughout the web page.

4) Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.
   
    > 1. Reduce the size of images to improve loading time and decrease data usage.
    > 2. Add `<meta name="viewport">` tag with `width` or `initial-scale` to optimize app for mobile screens.
    > 3. Preconnect to required origins in `<head>` to improve loading time, particularly to `fakestoreapi.com` and `https://fakestoreapi.com`.