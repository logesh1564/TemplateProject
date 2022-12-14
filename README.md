<!-- config pritter -->

step 1: Create file .prettierrc (root of the project)
step 2: Add Given Json
{
"trailingComma": "es5",
"tabWidth": 4,
"semi": false,
"singleQuote": true
}
for reference: https://prettier.io/docs/en/configuration.html

<!-- commitizen installation -->

step 1: use this command -> npm install -g commitizen
step 2: Add this line in package.json -> scripts -> "commit": "cz"
step 3: use this command - > commitizen init cz-conventional-changelog --save-dev --save-exact (OR) commitizen init cz-conventional-changelog --yarn --dev --exact
step 4: add the json  into package.json
   "config": {
        "commitizen": {
            "path": "cz-conventional-changelog"
        }
    }

for reference : https://www.npmjs.com/package/commitizen#making-your-repo-commitizen-friendly

<!-- Config commit Template -->

step 1: Create folder called .github
step 2: Inside the folder create File called PULL_REQUEST_TEMPLATE.md
step 3: inside that file add this

  <!-- start -->

## Pull request type (mark x wherever applicable, x is considered to be done)(Please try to limit your pull request to one type, submit multiple pull requests if needed.)

-   [ ] Bugfix
-   [ ] Feature
-   [ ] Code style update (formatting, renaming)
-   [ ] Refactoring (no functional changes, no api changes)
-   [ ] Build related changes
-   [ ] Documentation content changes
-   [ ] Performance

## JIRA/Linear Issue No

-

## Description (Clearly describe the detail of the work incorporated)

-

## Root cause (Briefly describe the root cause/analysi)

-

## Solution (Please describe the behavior or changes that are being added by this PR.)

-

## Impacted platform (mark x)

-   [ ] Web (Desktop)
-   [ ] Web (Mobile)

## Did you test the issue fix in all below browsers? (Applicable for websites)

-   [ ] Chrome
-   [ ] Firefox
-   [ ] Edge
-   [ ] Safari
-   [ ] Brave
-   [ ] Android chrome
-   [ ] iPhone Safari

## Any other information that is important to this PR such as screenshots of how the component looks before and after the change.

-

<!-- end -->
