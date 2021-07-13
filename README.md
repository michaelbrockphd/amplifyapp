# AmplifyApp

My attempt at following the [Amplify Tutorial](https://aws.amazon.com/getting-started/hands-on/build-react-app-amplify-graphql/) from Amazon.

## Notes

Turned out to be more challenging than planned.  While the exercise and concept was simple, sections of the tutorial are incomplete or out of date.

For example, readers may get stuck on [Module Two](https://aws.amazon.com/getting-started/hands-on/build-react-app-amplify-graphql/module-two/?e=gs2020&p=build-a-react-app-one) if following on Mac OS and have Safari as their default browser.  Safari will actively block some requests to localhost thus preventing the "amplify configure" command from completing.

Another sticking point was [Module Three](https://aws.amazon.com/getting-started/hands-on/build-react-app-amplify-graphql/module-three/?e=gs2020&p=build-a-react-app-two) where following the instructions will lead to build failures.

Thankfully a work around is [documented here](https://github.com/aws-amplify/amplify-cli/issues/6117).  In short, builds will initially fail as the wrong version of Amplify is being used on Amazon's side.

Additionally, one needs to make sure the front end [has the following role](https://docs.aws.amazon.com/amplify/latest/userguide/how-to-service-role-amplify-console.html) to deploy to the backend.

There are also numerous name typos (calling the backend dev instead of staging for example), but they are easy enough to work out.
