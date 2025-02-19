> **Much of the below is outdated based on the old repo that was last updated in 2016.  I'm in the midst of modernizing breakpoint based on developments in SASS over the last 5 years**

## Contributing to Breakpoint

We love contributors! Yes we do! If you would like to contribute to Breakpoint, please follow the following guidelines:

* **DO NOT ISSUE A PULL REQUEST WITHOUT RELATED ISSUE!!** All pull requests must reference an issue in the issue queue and will only be looked at after discussion about that issue has taken place. Any pull request created that does not reference an issue will be closed.
* All pull requests will be tested against our standard test suite through Travis CI. If any of the tests fail, we will ask you to fix your code so that the tests no longer fail. Any new features that are added must have accompanying passing tests before being considered. During a pull request, we may ask for additional tests to be written in order to ensure that what is being changed does not have negative effects elsewhere.
* We are actively trying to stay away from Ruby functionality and am attempting to build this entirely with native Sass functionality. If you would like to add a feature that includes Ruby code, there needs to be a very very compelling case as to why.
* Each individual feature you would like to add, or bug you would like to squash, should be an individual pull request. Each pull request should be from an individual feature branch to either the latest stable or development branch. **The current *stable* branch is 2.x.x. The current *development* branch is 2.x.x**. Contributions that are not in the form of a pull request will not be considered. If your pull request does not apply cleanly we will ask you to fix that before we will look into pulling it in. We may ask you to update or make changes to the code you've submitted, please don't take this the wrong way. If a pull request smells (such as if a large amount of code is all within a single commit, or the coding standards aren't in line with core Breakpoint) we may ask you to rewrite your commit.

### Testing

We have automated tests to ensure our build is working. To test, you must install [Bundler](http://bundler.io/), which will allow you to install all needed gem versions. Once you have Bundler up and running and have your dependencies installed, run ```bundle exec rake``` to run the tests. All tests are stored within the 'test' folder as .scss files. The test suite ensures that each test compiles, and does not change the expected behavior. If a test needs to be updated or changed, update the correct .scss file, and then run ```bundle exec rake compile``` to update all corrosponding css files.
