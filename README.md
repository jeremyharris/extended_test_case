# Extended Test Case

Extended test case aims to make the displeasure of using
`CakeTestCase::testAction()` slightly more pleasurable.

## Usage

Above your test case, use:

    App::import('Lib', 'ExtendedTestCase.ExtendedTestCase');

Then extend your test case with `ExtendedTestCase` instead of `CakeTestCase` and
define the `testController` variable in your test case as the controller you are
testing.

For more information about utilizing mocks, etc. visit [here][1].

## Features

- Falls back to old `testAction` method if `ExtendedTestCase::testController`
is not defined
- Allows use of mocks for things like the Email component or your controller
actions (render, header, etc.) in tests
- Simulates most of what the controller action does, minus actually rendering
anything

## License

Licensed under The MIT License
[http://www.opensource.org/licenses/mit-license.php][4]
Redistributions of files must retain the above copyright notice.

## Links

- [http://mark-story.com/posts/view/testing-cakephp-controllers-the-hard-way][2]
- [http://mark-story.com/posts/view/testing-cakephp-controllers-mock-objects-edition][3]
- [http://www.42pixels.com/blog/testing-controllers-the-slightly-less-hard-way][1]

[1]: http://www.42pixels.com/blog/testing-controllers-the-slightly-less-hard-way
[2]: http://mark-story.com/posts/view/testing-cakephp-controllers-the-hard-way
[3]: http://mark-story.com/posts/view/testing-cakephp-controllers-mock-objects-edition
[4]: http://www.opensource.org/licenses/mit-license.php