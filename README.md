# react-workshop
Repo to get started getting hands on with React

## step by step guide to get started

0. Clone this repo
```
git clone https://github.com/thaithcock/react-workshop.git
cd react-workshop
```

1. Set up create-react-app 

```
npx create-react-app .
```
2. Move our readme back (React has its own)
```
mv README.md README_REACT.md
mv README.old.md README.md
```
3. Verify create-react-app ran successfully
```
npm run start
```

4. Set up storybook
```
npx sb init
mkdir src/stories/examples
mv src/stories/assets src/stories/examples/
mv src/stories/*.* src/stories/examples/
```

5. Verifying storybook installed successfully
```
npm run storybook
```

6. Write a storybook file
```
# create ./src/stories/App.stories.jsx and paste this code:
import React from 'react';
import App from '../App';

export default {
  title: 'Workshop/App',
  component: App,
};

const Template = (args) => <App {...args} />;
export const Testing = Template.bind({});
```

7. Start react-ing!