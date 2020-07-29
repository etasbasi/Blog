---
title: How to setup testing with Redux, React Router, and Apollo GraphQL
layout: post
---

I recently had to write tests for a React app that used Redux, React Router and
Apollo Graphql. I first tried using enzyme to render the components, but couldn't get it
to work as intended, so I opted for the react-testing-library.

I took the example from [https://testing-library.com/docs/react-testing-library/setup](https://testing-library.com/docs/react-testing-library/setup)
and modified it to use apollo graphql test provider only if the `mocks` option is provided.

![code sample][sample-1]

And for testing the component:

![code sample][sample-2]

Hope this helps!

[sample-1]: {{site.url}}/Blog/images/post-assets/2020-07-29-1.png "Code Sample"
[sample-2]: {{site.url}}/Blog/images/post-assets/2020-07-29-2.png "Code Sample"