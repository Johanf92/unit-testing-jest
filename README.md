# unit-testing-jest

Learning about Unit testing code - JS - Jest

# describe()

In this example (apple.js) -> describe has been used to group assertions into a single block. The apple object needs to pass all three of these assertions. (apple.test.js) -> 1 failed

# it() vs test()

You may notice that we have swapped test() for it(). These are functionally identical, interchangeable and provided to help with readability.

Compare these two examples:

test("it shows a message when clicked", () => {
expect(...)
})

it("shows a message when clicked", () => {
expect(...)
})

They perform the same task but the second example is easier to read and understand when nested inside a describe statement.

# expect()

The expectations are set using expect() and each of these must succeed for the test to pass. There are a number of matchers that can be used to test the value of a variable or the result of a function.

Each data type (string, number, boolean, array, object, function, etc) has its own set of matchers in the same way that these types have different prototype methods in JavaScript.

expect(apple.color).toEqual("red");
expect(apple.texture).toEqual("juicy");
expect(apple.rating).toBeGreaterThan(6);
expect(apple.animalProduct).not.toBeTruthy();

1. Assuming that apple.color is a string, we can use the toEqual() matcher to check that it is equal to "red". Any other value will cause the test to fail.
   etc... etc... etc...

- any other value will cause the test to fail.

# Matchers

Matchers are functions that compare a value to an expected value. If a matcher succeeds, that assertion succeeds. As such, matchers are the atoms of Unit Testing.

- https://jestjs.io/docs/expect

The matchers we choose should:

    * Work for the type of value we expect
    * Check meaningful values about our code
    * Translate our test description into code

# Mocks
