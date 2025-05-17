# Lab 7

1) Where would you fit your automated tests in your Recipe project development pipeline? Select one of the following and explain why.

    a. Within a Github action that runs whenever code is pushed

    b. Manually run them locally before pushing code

    c. Run them all after all development is completed

    > I would fit my automated tests in the Recipe project development pipeline **within a Github action that runs whenever code is pushed**. This is because it ensures that every push that is made to a repository does not break the code. After each change, it ensures that the interactions with the localStorage, rendering, and component integration work as expected. For example, any change to `RecipeCard.js` or `main.js` could break the code (ex. rendering, event listeners, form behavior). Manually running tests locally before pushing code is less ideal because it is not enforced, it is inconsistent, and easy to forget. Running the tests after all development is complete is also not ideal before it will be very hard to find the bugs and issues in the code.